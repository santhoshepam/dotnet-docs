---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.CreateErrorWebPart(System.String,System.String,System.String,System.String,System.String)
additional_notes.overrides: *content
---

<p>If you want to customize the information that is returned in the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, you can override the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.CreateErrorWebPart(System.String,System.String,System.String,System.String,System.String)"></xref> method, call the base method, assign different values to the parameters passed to the base method, and then return the resulting <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control. For example, if you do not want end users to see the <code>originalPath</code> value (which would show the virtual directory path of a user control), when you call the base method you could pass an empty string ("") for that parameter.  
  
 You can also customize the behavior of the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control itself, by inheriting from it. For example, you might want to override its <xref href="System.Web.UI.WebControls.WebParts.Part.Title"></xref> or <xref href="System.Web.UI.WebControls.WebParts.WebPart.AllowMinimize"></xref> property.</p>


