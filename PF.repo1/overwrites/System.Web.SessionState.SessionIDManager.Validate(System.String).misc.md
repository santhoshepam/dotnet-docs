---
uid: System.Web.SessionState.SessionIDManager.Validate(System.String)
additional_notes.overrides: *content
---

<p>You can supply a custom session identifier to be used by ASP.NET session state by creating a class that inherits the <xref href="System.Web.SessionState.SessionIDManager"></xref> class and overriding the <xref href="System.Web.SessionState.SessionIDManager.CreateSessionID(System.Web.HttpContext)"></xref> and <xref href="System.Web.SessionState.SessionIDManager.Validate(System.String)"></xref> methods with your own custom implementation. Even when you create a custom session identifier, the session ID is limited to 80 characters by the <xref href="System.Web.SessionState.SessionIDManager"></xref> class.</p>


