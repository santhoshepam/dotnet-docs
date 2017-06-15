---
uid: System.ServiceModel.Channels.IDuplexSession.CloseOutputSession(System.TimeSpan)
additional_notes.overrides: *content
---

<p>
      <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> is a session method that can interact with the <xref href="System.ServiceModel.Channels.IDuplexSessionChannel"></xref> that owns the session. In particular, if your session lifetime is put together with your channel lifetime (like it is with TCP and reliable session and security):  
  
-   If <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> is called before <xref href="System.ServiceModel.ICommunicationObject.Close"></xref> is called on the channel, <xref href="System.ServiceModel.ICommunicationObject.Close"></xref> should wait for <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> to finish.  
  
-   If the channel is in the <xref href="System.ServiceModel.CommunicationState.Created"></xref> or <xref href="System.ServiceModel.CommunicationState.Opening"></xref> state, <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> should throw an <xref href="System.InvalidOperationException"></xref>.  
  
-   If the channel is in the <xref href="System.ServiceModel.CommunicationState.Faulted"></xref> state, <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> should throw a <xref href="System.ServiceModel.CommunicationObjectFaultedException"></xref>.  
  
-   The channel should fault if <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> throws.  
  
-   The implementation of <xref href="System.ServiceModel.ICommunicationObject.Close"></xref> on the channel should call <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> and then verify that <xref href="System.ServiceModel.Channels.IInputChannel.Receive"></xref> returns `null`, indicating that <xref href="System.ServiceModel.Channels.IDuplexSession.CloseOutputSession"></xref> was called from the other side of the session.</p>


