---
uid: System.Collections.Hashtable
thread_safety: *content
---

<xref href="System.Collections.Hashtable"></xref> is thread safe for use by multiple reader threads and a single writing thread. It is thread safe for multi-thread use when only one of the threads perform write (update) operations, which allows for lock-free reads provided that the writers are serialized to the <xref href="System.Collections.Hashtable"></xref>. To support multiple writers all operations on the <xref href="System.Collections.Hashtable"></xref> must be done through the wrapper returned by the <xref href="System.Collections.Hashtable.Synchronized(System.Collections.Hashtable)"></xref> method, provided that there are no threads reading the <xref href="System.Collections.Hashtable"></xref> object.  
  
 Enumerating through a collection is intrinsically not a thread safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


