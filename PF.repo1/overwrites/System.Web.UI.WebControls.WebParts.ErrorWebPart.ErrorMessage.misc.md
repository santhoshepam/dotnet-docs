---
uid: System.Web.UI.WebControls.WebParts.ErrorWebPart.ErrorMessage
additional_notes.overrides: *content
---

<p>Developers can assign a default value to the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.ErrorMessage"></xref> property by extending the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> class and, in the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.#ctor(System.String,System.String,System.String,System.String)"></xref> constructor or in an overridden <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.EndLoadPersonalization"></xref> method, assigning a default value to the property.  
  
 To require the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control to use a custom <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, you must also inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class and override its <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.CreateErrorWebPart(System.String,System.String,System.String,System.String,System.String)"></xref> method. In that method, you should assign the value of the method's <code>errorMessage</code> parameter to the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.ErrorMessage"></xref> property of your custom <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, because the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control calls this method from several other places, and usually passes in a specific error message.</p>


