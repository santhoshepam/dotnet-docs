---
uid: System.ComponentModel.AsyncCompletedEventArgs.Error
additional_notes.overrides: *content
---

<p>If you provide read-only properties in a derived class, be sure to call the <xref href="System.ComponentModel.AsyncCompletedEventArgs.RaiseExceptionIfNecessary"></xref> method in your property implementation. This prevents clients from accessing properties that are potentially not valid due to a failure in the asynchronous operation.</p>


