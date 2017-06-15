---
uid: System.ComponentModel.AsyncCompletedEventArgs.RaiseExceptionIfNecessary
additional_notes.overrides: *content
---

<p>If you have derived your own class from the <xref href="System.ComponentModel.AsyncCompletedEventArgs"></xref> class, your read-only properties should call the <xref href="System.ComponentModel.AsyncCompletedEventArgs.RaiseExceptionIfNecessary"></xref> method before returning the property value. If the component's asynchronous worker code assigns an exception to the <xref href="System.ComponentModel.AsyncCompletedEventArgs.Error"></xref> property or sets the <xref href="System.ComponentModel.AsyncCompletedEventArgs.Cancelled"></xref> property to `true`, the property will raise an exception if a client tries to read its value. This prevents clients from accessing properties that are potentially not valid due to a failure in the asynchronous operation.</p>


