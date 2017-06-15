---
summary: Creates a security binding element that expects clients to do certificate-based authentication using SOAP message security. This binding element expects the transport to provide server authentication as well as message protection (for example, HTTPS).
remarks: "The client must be configured with a certificate it uses for authentication.  \n  \n> [!NOTE]\n>  Once a <xref:System.ServiceModel.Channels.SecurityBindingElement> object is created by calling this method, the <xref:System.ServiceModel.Channels.SecurityBindingElement.MessageSecurityVersion%2A> property should be treated as immutable. Inconsistent binding behavior may occur if this value is modified."
uid: System.ServiceModel.Channels.SecurityBindingElement.CreateCertificateOverTransportBindingElement*
---
