---
uid: System.ComponentModel.AsyncOperation.PostOperationCompleted(System.Threading.SendOrPostCallback,System.Object)
additional_notes.overrides: *content
---

<p>Inheritors must make the <xref href="System.ComponentModel.AsyncOperation.PostOperationCompleted(System.Threading.SendOrPostCallback,System.Object)"></xref> invocation asynchronous, so that class library providers do not need to concern themselves with potential stack overflows if they assume asynchrony but a particular application model happens to be synchronous. The method should be interpreted as an "ending the lifetime" call, meaning the implementation needs to do what is appropriate for the application model. For instance, ASP.NET will decrement its count of outstanding asynchronous operations. This also should put the operation into a state such that any subsequent calls into it will fail, since it has now completed.  
  
 For more information about implementing asynchronous classes, see [Implementing the Event-based Asynchronous Pattern](~/docs/standard/asynchronous-programming-patterns/implementing-the-event-based-asynchronous-pattern.md).</p>


