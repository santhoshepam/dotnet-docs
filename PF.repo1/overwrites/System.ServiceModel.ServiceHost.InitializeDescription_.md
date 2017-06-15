---
summary: Initializes a description of the service hosted based on its type or instance.
remarks: This method removes the requirement for passing base addresses as part of <xref:System.ServiceModel.ServiceHost.%23ctor%2A>. Classes that inherit from <xref:System.ServiceModel.ServiceHost> can call <xref:System.ServiceModel.ServiceHost.%23ctor%2A> and then can call one of the <xref:System.ServiceModel.ServiceHost.InitializeDescription%2A> when a base address is available. This is how the Service Model Metadata Utility Tool (Svcutil.exe) is implemented.
uid: System.ServiceModel.ServiceHost.InitializeDescription*
---
