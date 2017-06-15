---
uid: System.Collections.Concurrent.Partitioner`1
thread_safety: *content
---

The static methods on <xref href="System.Collections.Concurrent.Partitioner`1"></xref> are all thread-safe and may be used concurrently from multiple threads. However, while a created partitioner is in use, the underlying data source should not be modified, whether from the same thread that is using a partitioner or from a separate thread.


