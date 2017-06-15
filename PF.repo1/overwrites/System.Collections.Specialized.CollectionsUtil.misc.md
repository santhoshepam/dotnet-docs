---
uid: System.Collections.Specialized.CollectionsUtil
thread_safety: *content
---

A <xref href="System.Collections.Hashtable"></xref> can support one writer and multiple readers concurrently. To support multiple writers, all operations must be done through the wrapper returned by the <xref href="System.Collections.Hashtable.Synchronized(System.Collections.Hashtable)"></xref> method.  
  
 A <xref href="System.Collections.SortedList"></xref> can support multiple readers concurrently, as long as the collection is not modified. To guarantee the thread safety of the <xref href="System.Collections.SortedList"></xref>, all operations must be done through the wrapper returned by the <xref href="System.Collections.SortedList.Synchronized(System.Collections.SortedList)"></xref> method.  
  
 Enumerating through a collection is intrinsically not a thread safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


