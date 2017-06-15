---
uid: System.Collections.Generic.LinkedList`1
thread_safety: *content
---

This type is not thread safe. If the <xref href="System.Collections.Generic.LinkedList`1"></xref> needs to be accessed by multiple threads, you will need to implement their own synchronization mechanism.  
  
 A <xref href="System.Collections.Generic.LinkedList`1"></xref> can support multiple readers concurrently, as long as the collection is not modified. Even so, enumerating through a collection is intrinsically not a thread-safe procedure. In the rare case where an enumeration contends with write accesses, the collection must be locked during the entire enumeration. To allow the collection to be accessed by multiple threads for reading and writing, you must implement your own synchronization.


