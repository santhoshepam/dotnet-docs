---
summary: Runs a query against the message and returns a value that satisfies the query.
remarks: The difference between the two overloads is that one takes a <xref:System.ServiceModel.Channels.Message> parameter and is not permitted to examine the body. The other takes a <xref:System.ServiceModel.Channels.MessageBuffer> parameter and can examine any part of the message. Message headers are automatically buffered and can be queried without being consumed. However, if the body is to be queried, then the entire message must be buffered because an unbuffered message body can be consumed by the query.
uid: System.ServiceModel.Dispatcher.MessageQueryCollection.Evaluate``1*
---
