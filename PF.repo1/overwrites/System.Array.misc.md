---
uid: System.Array
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 This implementation does not provide a synchronized (thread safe) wrapper for an <xref href="System.Array"></xref>; however, .NET Framework classes based on <xref href="System.Array"></xref> provide their own synchronized version of the collection using the <xref href="System.Array.SyncRoot"></xref> property.  
  
 Enumerating through a collection is intrinsically not a thread-safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


