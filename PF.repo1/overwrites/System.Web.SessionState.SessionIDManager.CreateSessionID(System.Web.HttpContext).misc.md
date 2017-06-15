---
uid: System.Web.SessionState.SessionIDManager.CreateSessionID(System.Web.HttpContext)
additional_notes.overrides: *content
---

<p>You can supply a custom session identifier to be used by ASP.NET session state by creating a class that inherits the <xref href="System.Web.SessionState.SessionIDManager"></xref> class and overriding the <xref href="System.Web.SessionState.SessionIDManager.CreateSessionID(System.Web.HttpContext)"></xref> and <xref href="System.Web.SessionState.SessionIDManager.Validate(System.String)"></xref> methods with your own custom implementations. If your custom session ID does not meet the character constraints enforced by the default implementation of the <xref href="System.Web.SessionState.SessionIDManager.Validate(System.String)"></xref> method, you should override the <xref href="System.Web.SessionState.SessionIDManager.Validate(System.String)"></xref> method to provide validation of your custom session identifier. In this case, the <xref href="System.Web.SessionState.SessionIDManager"></xref> class will ensure that your custom session identifier is URL encoded in the HTTP response and URL decoded from the HTTP request using the <xref href="System.Web.SessionState.SessionIDManager.Encode(System.String)"></xref> and <xref href="System.Web.SessionState.SessionIDManager.Decode(System.String)"></xref> methods, respectively.</p>


