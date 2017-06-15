---
uid: System.Threading.ManualResetEventSlim
thread_safety: *content
---

All public and protected members of <xref href="System.Threading.ManualResetEventSlim"></xref> are thread-safe and may be used concurrently from multiple threads, with the exception of Dispose, which must only be used when all other operations on the <xref href="System.Threading.ManualResetEventSlim"></xref> have completed, and Reset, which should only be used when no other threads are accessing the event.


