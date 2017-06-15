---
uid: System.ComponentModel.AsyncOperation
additional_notes.overrides: *content
---

<p>Implementers must ensure the <xref href="System.ComponentModel.AsyncOperation.PostOperationCompleted(System.Threading.SendOrPostCallback,System.Object)"></xref> and <xref href="System.ComponentModel.AsyncOperation.Post(System.Threading.SendOrPostCallback,System.Object)"></xref> invocations are asynchronous, so that class library providers do not need to concern themselves with potential stack overflows if they assume asynchronous behavior in a particular application model that happens to be synchronous.  
  
 For more information about implementing asynchronous classes, see [Implementing the Event-based Asynchronous Pattern](~/docs/standard/asynchronous-programming-patterns/implementing-the-event-based-asynchronous-pattern.md).</p>


