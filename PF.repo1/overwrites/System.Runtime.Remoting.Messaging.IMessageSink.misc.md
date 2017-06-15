---
uid: System.Runtime.Remoting.Messaging.IMessageSink
additional_notes.overrides: *content
---

<p>It is important to note that code implementing the current interface must provide implementations for both <xref href="System.Runtime.Remoting.Messaging.IMessageSink.SyncProcessMessage(System.Runtime.Remoting.Messaging.IMessage)"></xref> and <xref href="System.Runtime.Remoting.Messaging.IMessageSink.AsyncProcessMessage(System.Runtime.Remoting.Messaging.IMessage,System.Runtime.Remoting.Messaging.IMessageSink)"></xref>, since synchronous calls can be converted to asynchronous calls and vice versa. Both methods must be implemented, even if the sink does not support asynchronous processing.</p>


