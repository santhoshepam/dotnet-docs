---
summary: Attempts to disallow garbage collection during the execution of a critical path.
remarks: >-
  > [!IMPORTANT]

  >  You cannot nest calls to the <xref:System.GC.TryStartNoGCRegion%2A> method, and you should only call the <xref:System.GC.EndNoGCRegion%2A> method if the runtime is currently in no GC region latency mode. In other words, you should not call <xref:System.GC.TryStartNoGCRegion%2A> multiple times (after the first method call, subsequent calls will not succeed), and you should not expect calls to <xref:System.GC.EndNoGCRegion%2A> to succeed just because the first call to <xref:System.GC.TryStartNoGCRegion%2A> succeeded.
uid: System.GC.TryStartNoGCRegion*
---
