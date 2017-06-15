---
summary: Provides a managed wrapper for the IIS method that inserts an HTTP request entity body into memory.
remarks: "The <xref:System.Web.HttpRequest.InsertEntityBody%2A> method overloads provide managed access to the IIS 7 `IHttpRequest::InsertEntityBody` method. The IIS method inserts an HTTP request entity body (the data that is posted by a client) into memory. This is useful because IIS does not maintain a copy of the request entity after it has been read. The <xref:System.Web.HttpRequest.InsertEntityBody%2A> methods create a copy of the HTTP request entity data and make it available to IIS for additional custom handling.  \n  \n> [!NOTE]\n>  The <xref:System.Web.HttpRequest.InsertEntityBody%2A> method overloads work only on IIS 7.0 or later, because the `IHttpRequest::InsertEntityBody` method was added in IIS 7.0."
uid: System.Web.HttpRequest.InsertEntityBody*
---
