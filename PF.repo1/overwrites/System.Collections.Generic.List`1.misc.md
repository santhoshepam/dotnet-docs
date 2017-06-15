---
uid: System.Collections.Generic.List`1
thread_safety: *content
---

Public static (`Shared` in Visual Basic) members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 It is safe to perform multiple read operations on a <xref href="System.Collections.Generic.List`1"></xref>, but issues can occur if the collection is modified while it’s being read. To ensure thread safety, lock the collection during a read or write operation. To enable a collection to be accessed by multiple threads for reading and writing, you must implement your own synchronization. For collections with built-in synchronization, see the classes in the <xref href="System.Collections.Concurrent"></xref> namespace. For an inherently thread–safe alternative, see the <xref href="System.Collections.Immutable.ImmutableList`1"></xref> class.


