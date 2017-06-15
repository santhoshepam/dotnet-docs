---
uid: System.Collections.Queue
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 To guarantee the thread safety of the <xref href="System.Collections.Queue"></xref>, all operations must be done through the wrapper returned by the <xref href="System.Collections.Queue.Synchronized(System.Collections.Queue)"></xref> method.  
  
 Enumerating through a collection is intrinsically not a thread-safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


