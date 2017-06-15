---
summary: When overridden in a derived class, tests whether a message or a buffered message satisfies the criteria of a filter.
remarks: "The difference between the two overloads is that one takes a <xref:System.ServiceModel.Channels.Message> parameter and is not permitted to examine the body. The other takes a <xref:System.ServiceModel.Channels.MessageBuffer> parameter and can examine any part of the message. Message headers are automatically buffered and can be inspected by a filter without being consumed. But if the body is to be inspected by a filter, then the entire message must be buffered because an unbuffered message body can be consumed by a query and its contents destroyed.  \n  \n Use <xref:System.ServiceModel.Dispatcher.MessageFilter.Match%2A> if examination of the body is not required. Use <xref:System.ServiceModel.Dispatcher.MessageFilter.Match%2A> if examination of the message body is required."
uid: System.ServiceModel.Dispatcher.MessageFilter.Match*
---
