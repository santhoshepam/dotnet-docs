---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.IsAuthorized(System.Type,System.String,System.String,System.Boolean)
additional_notes.overrides: *content
---

<p>This method can be overridden by inheriting from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class, if you want to provide additional handling when checking authorization. You might want to override the method to check for certain values in the <code>authorizationFilter</code> parameter, and based on the value, return a Boolean value that determines whether the control will be added to a page.  
  
 For page developers who also want to check for authorization filters and provide custom handling, there is an option for doing this inline in an .aspx page, or in a code-behind file, without having to inherit from any classes. You can declare an alternate event handler in the page for the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.OnAuthorizeWebPart(System.Web.UI.WebControls.WebParts.WebPartAuthorizationEventArgs)"></xref> method of the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control. For more details and an example, see the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.OnAuthorizeWebPart(System.Web.UI.WebControls.WebParts.WebPartAuthorizationEventArgs)"></xref> method.</p>


