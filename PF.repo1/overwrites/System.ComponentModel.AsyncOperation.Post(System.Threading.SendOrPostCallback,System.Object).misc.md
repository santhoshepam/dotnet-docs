---
uid: System.ComponentModel.AsyncOperation.Post(System.Threading.SendOrPostCallback,System.Object)
additional_notes.overrides: *content
---

<p>Inheritors must make the <xref href="System.ComponentModel.AsyncOperation.Post(System.Threading.SendOrPostCallback,System.Object)"></xref> invocation asynchronous, so that class library providers do not need to concern themselves with potential stack overflows if they assume asynchrony but a particular application model happens to be synchronous.  
  
 <block subset="none" type="note"><p>  
 Console applications do not synchronize the execution of <xref href="System.ComponentModel.AsyncOperation.Post(System.Threading.SendOrPostCallback,System.Object)"></xref> calls. This can cause `ProgressChanged` events to be raised out of order. If you wish to have serialized execution of <xref href="System.ComponentModel.AsyncOperation.Post(System.Threading.SendOrPostCallback,System.Object)"></xref> calls, implement and install a <xref href="System.Threading.SynchronizationContext"></xref> class.  
  
</p></block>  
  
 For more information about implementing asynchronous classes, see [Implementing the Event-based Asynchronous Pattern](~/docs/standard/asynchronous-programming-patterns/implementing-the-event-based-asynchronous-pattern.md).</p>


