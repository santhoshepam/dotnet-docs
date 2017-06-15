---
summary: Begins an asynchronous receive operation.
remarks: Use the asynchronous <xref:System.ServiceModel.Channels.IInputChannel.BeginReceive%2A> method when you want the application processing to continue without waiting for the request to be received. Use the synchronous <xref:System.ServiceModel.Channels.IInputChannel.Receive%2A> method when it is acceptable for the current thread to be blocked until the request message is received or the interval of time specified by the `timeout` has been exceeded. The asynchronous operation is available with or without an explicit timeout.
uid: System.ServiceModel.Channels.IInputChannel.BeginReceive*
---
