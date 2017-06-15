---
summary: Retrieves the body of this <xref href="System.ServiceModel.Channels.Message"></xref> instance.
remarks: "After a message is created, the message body can be read using the <xref:System.ServiceModel.Channels.Message.GetBody%2A> methods on the returned message. The returned object encapsulates all the child elements within the `Body` element. Because the body of a message is a stream, it can only be written once, or read once.  \n  \n Use the <xref:System.ServiceModel.Channels.Message.GetBody%60%601%28System.Runtime.Serialization.XmlObjectSerializer%29> overload when working with JSON messages; the <xref:System.ServiceModel.Channels.Message.GetBody%60%601> overload does not work."
example:
- "The following code example shows a client that uses the channel factory to send a message and read the reply.  \n  \n [!code-csharp[Message#0](~/samples/snippets/csharp/VS_Snippets_CFX/message/cs/client.cs#0)]\n [!code-vb[Message#0](~/samples/snippets/visualbasic/VS_Snippets_CFX/message/vb/client.vb#0)]"
uid: System.ServiceModel.Channels.Message.GetBody``1*
---
