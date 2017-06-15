---
uid: System.Web.UI.WebControls.WebParts.ErrorWebPart.AddAttributesToRender(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>This method can be overridden in a derived <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> class, if developers want to customize the style characteristics that are applied to an <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control.  
  
 To require the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control to use a custom <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, you must also inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class and override its <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.CreateErrorWebPart(System.String,System.String,System.String,System.String,System.String)"></xref> method. In that method, you should assign the value of the method's <code>errorMessage</code> parameter to the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.ErrorMessage"></xref> property of your custom <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, because the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control calls this method from several other places, and usually passes in a specific error message.</p>


