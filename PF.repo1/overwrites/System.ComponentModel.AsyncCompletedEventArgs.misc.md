---
uid: System.ComponentModel.AsyncCompletedEventArgs
additional_notes.overrides: *content
---

<p>Classes that follow the Event-based Asynchronous Pattern can raise events to alert clients about the status of pending asynchronous operations. If the class provides a *MethodName*`Completed` event, you can use the <xref href="System.ComponentModel.AsyncCompletedEventArgs"></xref> to tell clients about the outcome of asynchronous operations.  
  
 You may want to communicate to clients more information about the outcome of an asynchronous operation than an <xref href="System.ComponentModel.AsyncCompletedEventArgs"></xref> accommodates. In this case, you can derive your own class from the <xref href="System.ComponentModel.AsyncCompletedEventArgs"></xref> class and provide additional private instance variables and corresponding read-only public properties. Call the <xref href="System.ComponentModel.AsyncCompletedEventArgs.RaiseExceptionIfNecessary"></xref> method before returning the property value, in case the operation was canceled or an error occurred.</p>


