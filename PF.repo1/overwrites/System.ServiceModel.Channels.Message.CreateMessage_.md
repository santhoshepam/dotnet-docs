---
summary: Creates a message.
remarks: "This method is used to create a new copy of a message ready for sending.  \n  \n When working with JSON messages use the <xref:System.ServiceModel.Channels.Message.CreateMessage%28System.ServiceModel.Channels.MessageVersion%2CSystem.String%2CSystem.Object%2CSystem.Runtime.Serialization.XmlObjectSerializer%29> method, the <xref:System.ServiceModel.Channels.Message.CreateMessage%28System.ServiceModel.Channels.MessageVersion%2CSystem.String%2CSystem.Object%29> method does not work with JSON messages."
example:
- "The following code example shows a client that uses the channel factory to send a message and read the reply.  \n  \n [!code-csharp[Message#0](~/samples/snippets/csharp/VS_Snippets_CFX/message/cs/client.cs#0)]\n [!code-vb[Message#0](~/samples/snippets/visualbasic/VS_Snippets_CFX/message/vb/client.vb#0)]"
uid: System.ServiceModel.Channels.Message.CreateMessage*
---
