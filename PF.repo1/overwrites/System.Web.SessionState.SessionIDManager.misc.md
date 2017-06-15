---
uid: System.Web.SessionState.SessionIDManager
additional_notes.overrides: *content
---

<p>You can replace the ASP.NET session identifier with your own custom session identifier by creating a class that inherits the <xref href="System.Web.SessionState.SessionIDManager"></xref> class and overriding the <xref href="System.Web.SessionState.SessionIDManager.CreateSessionID(System.Web.HttpContext)"></xref> and <xref href="System.Web.SessionState.SessionIDManager.Validate(System.String)"></xref> methods with your own custom implementations. For an example of overriding the <xref href="System.Web.SessionState.SessionIDManager"></xref> class and implementing these methods, see the example provided for the <xref href="System.Web.SessionState.SessionIDManager.CreateSessionID(System.Web.HttpContext)"></xref> method.  
  
 You can replace the entire <xref href="System.Web.SessionState.SessionIDManager"></xref> with a custom session-ID manager by creating a class that implements the <xref href="System.Web.SessionState.ISessionIDManager"></xref> interface. If your custom session-ID manager supports cookieless session identifiers, you will need to implement a solution for sending and retrieving session identifiers in the URL, such as an ISAPI filter. For more information about creating a custom session-ID manager, see <xref href="System.Web.SessionState.ISessionIDManager"></xref>.</p>


