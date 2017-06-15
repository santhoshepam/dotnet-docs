---
uid: System.ServiceModel.Dispatcher.IMessageFilterTable`1.GetMatchingFilter(System.ServiceModel.Channels.Message,System.ServiceModel.Dispatcher.MessageFilter@)
additional_notes.overrides: *content
---

<p>If more than one filter matches the message, a <xref href="System.ServiceModel.Dispatcher.MultipleFilterMatchesException"></xref> must be thrown.  
  
 This version takes a <xref href="System.ServiceModel.Channels.Message"></xref> and must throw an <xref href="System.ServiceModel.Dispatcher.InvalidBodyAccessException"></xref> if it tries to examine the message body.</p>


