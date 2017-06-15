---
uid: System.Collections.DictionaryBase
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 This implementation does not provide a synchronized (thread-safe) wrapper for a <xref href="System.Collections.DictionaryBase"></xref>, but derived classes can create their own synchronized versions of the <xref href="System.Collections.DictionaryBase"></xref> using the <xref href="System.Collections.ICollection.SyncRoot"></xref> property.  
  
 Enumerating through a collection is intrinsically not a thread-safe procedure. Even when a collection is synchronized, other threads can still modify the collection, which causes the enumerator to throw an exception. To guarantee thread safety during enumeration, you can either lock the collection during the entire enumeration or catch the exceptions resulting from changes made by other threads.


---
uid: System.Collections.DictionaryBase
additional_notes.overrides: *content
---

<p>This base class is provided to make it easier for implementers to create a strongly typed custom collection. Implementers are encouraged to extend this base class instead of creating their own.  
  
 Members of this base class are protected and are intended to be used through a derived class only.</p>


