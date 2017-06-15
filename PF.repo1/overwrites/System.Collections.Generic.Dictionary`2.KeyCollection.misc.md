---
uid: System.Collections.Generic.Dictionary`2.KeyCollection
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 A <xref href="System.Collections.Generic.Dictionary`2.KeyCollection"></xref> can support multiple readers concurrently, as long as the collection is not modified.  Even so, enumerating through a collection is intrinsically not a thread-safe procedure.  To guarantee thread safety during enumeration, you can lock the collection during the entire enumeration.  To allow the collection to be accessed by multiple threads for reading and writing, you must implement your own synchronization.


