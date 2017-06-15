---
summary: Tests whether a message or buffered message satisfies the criteria of the endpoint filter.
remarks: "The difference between the two overloads of the <xref:System.ServiceModel.Dispatcher.EndpointAddressMessageFilter.Match%2A> method is that the one that takes the <xref:System.ServiceModel.Channels.MessageBuffer> parameter is permitted to examine the body of a message when testing for a match, while the one that takes the <xref:System.ServiceModel.Channels.Message> parameter is not.  \n  \n <xref:System.ServiceModel.Dispatcher.EndpointAddressMessageFilter.Match%2A> does not test the contents of the body of a message, so these two methods are equivalent."
uid: System.ServiceModel.Dispatcher.EndpointAddressMessageFilter.Match*
---
