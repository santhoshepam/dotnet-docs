---
summary: Tests whether a message or a buffered message matches one of the actions configured for the filter.
remarks: "The difference between the two overloads is that one takes a <xref:System.ServiceModel.Channels.Message> parameter and cannot examine the message body; the other takes a <xref:System.ServiceModel.Channels.MessageBuffer> parameter and can examine any part of the message.  Because an action filter does not examine the body, these methods are equivalent.  \n  \n If you must check the message against multiple <xref:System.ServiceModel.Dispatcher.ActionMessageFilter> objects, put the filters into an <xref:System.ServiceModel.Dispatcher.IMessageFilterTable%601> and then use the matching functionality provided by the table."
uid: System.ServiceModel.Dispatcher.ActionMessageFilter.Match*
---
