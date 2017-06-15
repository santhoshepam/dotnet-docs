---
uid: System.Web.Services.Protocols.HttpWebClientProtocol
thread_safety: *content
---

The properties on this class are copied into a new instance of a <xref href="System.Net.WebRequest"></xref> object for each XML Web service method call. While you can call XML Web service methods on the same <xref href="System.Web.Services.Protocols.WebClientProtocol"></xref> instance from different threads at the same time, there is no synchronization done to ensure that a consistent snapshot of the properties gets transferred to the <xref href="System.Net.WebRequest"></xref> object. Therefore, if you need to modify the properties and make concurrent method calls from different threads you should use a different instance of the XML Web service proxy or provide your own synchronization.


