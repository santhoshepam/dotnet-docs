---
summary: Returns a value that indicates whether the current binding can build a channel factory stack on the client that satisfies some specific criteria.
remarks: Use this method if you want to check that the channel factory for channels of type `TChannel` can be build for the `context` provided before attempting to actually build the factory. Alternatively, try to build the channel factory by calling <xref:System.ServiceModel.Channels.BindingElement.BuildChannelFactory%2A> and catch the exception generated if it cannot be built.
uid: System.ServiceModel.Channels.Binding.CanBuildChannelFactory``1*
---
