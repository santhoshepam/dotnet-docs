---
uid: System.Web.UI.WebControls.WebParts.ErrorWebPart
additional_notes.overrides: *content
---

<p>The conditions in which an <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control is actually inserted into a page are relatively rare, and although the class can be inherited from and extended, few developers will find this to be of great importance. One reason you might want to extend this class is if you want to customize the appearance and behavior of the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control. For example, you could override the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.EndLoadPersonalization"></xref> method, and set additional style or other properties on the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, beyond those that are already set.  
  
 To require the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control to use a custom <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, you must also inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class and override its <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.CreateErrorWebPart(System.String,System.String,System.String,System.String,System.String)"></xref> method. In that method, you should assign the value of the method's <code>errorMessage</code> parameter to the <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart.ErrorMessage"></xref> property of your custom <xref href="System.Web.UI.WebControls.WebParts.ErrorWebPart"></xref> control, because the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control calls this method from several other places, and often passes in a different error message value.</p>


