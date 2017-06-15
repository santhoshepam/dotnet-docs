---
summary: Causes a communication object to transition from the created state into the opened state.
remarks: When called, the <xref:System.ServiceModel.Channels.CommunicationObject.Open%2A> method causes a <xref:System.ServiceModel.Channels.CommunicationObject> to enter into the <xref:System.ServiceModel.CommunicationState.Opening> state and calls <xref:System.ServiceModel.Channels.CommunicationObject.OnOpening%2A>, <xref:System.ServiceModel.Channels.CommunicationObject.Open%2A>, and <xref:System.ServiceModel.Channels.CommunicationObject.OnOpened%2A>.  The <xref:System.ServiceModel.Channels.CommunicationObject.OnOpened%2A> method completes the <xref:System.ServiceModel.Channels.CommunicationObject.Open%2A> method by setting the state of the object to the <xref:System.ServiceModel.CommunicationState.Opened> state.
uid: System.ServiceModel.Channels.CommunicationObject.Open*
---
