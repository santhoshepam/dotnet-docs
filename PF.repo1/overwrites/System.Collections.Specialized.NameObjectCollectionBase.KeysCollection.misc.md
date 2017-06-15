---
uid: System.Collections.Specialized.NameObjectCollectionBase.KeysCollection
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 This implementation does not provide a synchronized (thread safe) wrapper for a <xref href="System.Collections.Specialized.NameObjectCollectionBase.KeysCollection"></xref>, but derived classes can create their own synchronized versions of the <xref href="System.Collections.Specialized.NameObjectCollectionBase.KeysCollection"></xref> using the <xref href="System.Collections.ICollection.SyncRoot"></xref> property.  
  
 Enumerating through a collection is intrinsically not a thread-safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


