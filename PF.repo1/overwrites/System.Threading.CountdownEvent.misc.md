---
uid: System.Threading.CountdownEvent
thread_safety: *content
---

All public and protected members of <xref href="System.Threading.CountdownEvent"></xref> are thread-safe and may be used concurrently from multiple threads, with the exception of Dispose, which must only be used when all other operations on the <xref href="System.Threading.CountdownEvent"></xref> have completed, and Reset, which should only be used when no other threads are accessing the event.  
  
 Example  
  
 The following example shows how to use a <xref href="System.Threading.CountdownEvent"></xref>:  
  
 [!code-csharp[System.Threading.CountdownEvent#01](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.threading.countdownevent/cs/countdownevent.cs#01)]
 [!code-vb[System.Threading.CountdownEvent#01](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.threading.countdownevent/vb/countdownevent.vb#01)]


