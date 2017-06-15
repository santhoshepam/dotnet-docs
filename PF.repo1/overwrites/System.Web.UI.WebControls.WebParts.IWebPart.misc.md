---
uid: System.Web.UI.WebControls.WebParts.IWebPart
additional_notes.overrides: *content
---

<p>Normally you do not need to implement the <xref href="System.Web.UI.WebControls.WebParts.IWebPart"></xref> interface, either on custom <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> controls or server controls, because the base <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> class already implements the interface. Custom <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> controls, and other server controls that are placed in <xref href="System.Web.UI.WebControls.WebParts.WebPartZoneBase"></xref> zones, can use all the <xref href="System.Web.UI.WebControls.WebParts.IWebPart"></xref> properties.  
  
 The main reason to implement the <xref href="System.Web.UI.WebControls.WebParts.IWebPart"></xref> interface yourself, whether in a custom <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control or another server control, is if you want to change the default implementation. For example, you might want to provide default values for some of the properties. Another reason to implement the interface in a user or server control is so that the design-time experience of working with these properties on the control will be enhanced.</p>


