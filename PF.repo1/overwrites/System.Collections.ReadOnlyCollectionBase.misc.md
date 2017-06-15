---
uid: System.Collections.ReadOnlyCollectionBase
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 This implementation does not provide a synchronized (thread safe) wrapper for a <xref href="System.Collections.ReadOnlyCollectionBase"></xref>, but derived classes can create their own synchronized versions of the <xref href="System.Collections.ReadOnlyCollectionBase"></xref> using the <xref href="System.Collections.ICollection.SyncRoot"></xref> property.  
  
 Enumerating through a collection is intrinsically not a thread-safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


---
uid: System.Collections.ReadOnlyCollectionBase
additional_notes.overrides: *content
---

<p>This base class is provided to make it easier for implementers to create a strongly typed read-only custom collection. Implementers are encouraged to extend this base class instead of creating their own. Members of this base class are protected and are intended to be used through a derived class only.  
  
 This class makes the underlying collection available through the <xref href="System.Collections.ReadOnlyCollectionBase.InnerList"></xref> property, which is intended for use only by classes that are derived directly from <xref href="System.Collections.ReadOnlyCollectionBase"></xref>. The derived class must ensure that its own users cannot modify the underlying collection.</p>


