---
summary: Returns a message received by the input channel, if one is available with an interval of time that is explicitly or implicitly defined.
remarks: "Use the synchronous <xref:System.ServiceModel.Channels.IInputChannel.Receive%2A> method when it is acceptable for the current thread to be blocked until it receives the request message or exceeds the interval of time specified by `timeout`. Use the asynchronous <xref:System.ServiceModel.Channels.IInputChannel.BeginReceive%2A> method when you need the application processing to continue without waiting for the request to be received.  \n  \n The synchronous <xref:System.ServiceModel.Channels.IInputChannel.Receive%2A> operation is available with or without an explicit timeout.  \n  \n If a message is not available, it blocks until one is available or until the timeout is exceeded."
uid: System.ServiceModel.Channels.IInputChannel.Receive*
---
