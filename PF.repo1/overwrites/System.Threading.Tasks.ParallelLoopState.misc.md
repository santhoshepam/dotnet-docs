---
uid: System.Threading.Tasks.ParallelLoopState
thread_safety: *content
---

A <xref href="System.Threading.Tasks.ParallelLoopState"></xref> instance is meant to be used only within the body of the loop to which an instance was provided.  It is not safe to use a provided <xref href="System.Threading.Tasks.ParallelLoopState"></xref> instance after the associated loop ends, nor is it safe to explicitly hand it off to other threads and have those threads access it at any time.  A different <xref href="System.Threading.Tasks.ParallelLoopState"></xref> instance will be provided to each thread involved in a loop.


