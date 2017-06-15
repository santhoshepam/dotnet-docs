---
uid: System.Web.Services.Protocols.SoapHttpClientProtocol
thread_safety: *content
---

This type is thread safe.


---
uid: System.Web.Services.Protocols.SoapHttpClientProtocol
additional_notes.overrides: *content
---

<p>When you override this class, you can introduce methods in the derived class which are specific to a particular type of XML Web service. The methods capture the parameters and call the base class to do the work of communicating with the XML Web service. If the introduced methods are asynchronous, call the <xref href="System.Web.Services.Protocols.SoapHttpClientProtocol.BeginInvoke(System.String,System.Object[],System.AsyncCallback,System.Object)"></xref> method and the <xref href="System.Web.Services.Protocols.SoapHttpClientProtocol.EndInvoke(System.IAsyncResult)"></xref> method. If the introduced methods are synchronous, call the <xref href="System.Web.Services.Protocols.SoapHttpClientProtocol.Invoke(System.String,System.Object[])"></xref> method. The overridden constructor typically sets the <xref href="System.Web.Services.Protocols.WebClientProtocol.Url"></xref> property to the URL of the XML Web service method.</p>


