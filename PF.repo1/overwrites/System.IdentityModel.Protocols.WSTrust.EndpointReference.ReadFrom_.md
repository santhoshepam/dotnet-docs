---
summary: Reads an wsa:EndpointReference element from the specified reader.
remarks: Reads the contents of the wsa:EndpointReference element and returns an <xref:System.IdentityModel.Protocols.WSTrust.EndpointReference> object. The WS-Addressing namespace can be either the WS-Addressing standard schema (http://schemas.xmlsoap.org/ws/2004/08/addressing) or the WS-Addressing 1.0 standard schema (http://www.w3.org/2005/08/addressing). The wsa:Address element must be the first child element of the wsa:EndpointReference element. The <xref:System.IdentityModel.Protocols.WSTrust.EndpointReference.Uri%2A> property in the returned <xref:System.IdentityModel.Protocols.WSTrust.EndpointReference> is set to the URI specified by the wsa:Address element. All other child elements are added to the <xref:System.IdentityModel.Protocols.WSTrust.EndpointReference.Details%2A> collection.
uid: System.IdentityModel.Protocols.WSTrust.EndpointReference.ReadFrom*
---
