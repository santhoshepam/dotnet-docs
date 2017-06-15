---
uid: System.Web.UI.WebControls.Login.Authenticate
additional_notes.overrides: *content
---

<p>Custom authentication schemes should set the <xref href="System.Web.UI.WebControls.AuthenticateEventArgs.Authenticated"></xref> property to `true` to indicate that a user has been authenticated.  
  
 When a user submits his or her login information, the <xref href="System.Web.UI.WebControls.Login"></xref> control first raises the <xref href="System.Web.UI.WebControls.Login.LoggingIn"></xref> event, then the <xref href="System.Web.UI.WebControls.Login.Authenticate"></xref> event, and finally the <xref href="System.Web.UI.WebControls.Login.LoggedIn"></xref> event.</p>


