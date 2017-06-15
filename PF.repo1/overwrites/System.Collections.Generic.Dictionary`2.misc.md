---
uid: System.Collections.Generic.Dictionary`2
thread_safety: *content
---

A <xref href="System.Collections.Generic.Dictionary`2"></xref> can support multiple readers concurrently, as long as the collection is not modified. Even so, enumerating through a collection is intrinsically not a thread-safe procedure. In the rare case where an enumeration contends with write accesses, the collection must be locked during the entire enumeration. To allow the collection to be accessed by multiple threads for reading and writing, you must implement your own synchronization.  
  
 For thread-safe alternatives, see the <xref href="System.Collections.Concurrent.ConcurrentDictionary`2"></xref> class or <xref href="System.Collections.Immutable.ImmutableDictionary`2"></xref> class.  
  
 Public static (`Shared` in Visual Basic) members of this type are thread safe.


