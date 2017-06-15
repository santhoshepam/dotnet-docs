---
uid: System.Web.UI.Design.WebControls.LoginNameDesigner.UsePreviewControl
additional_notes.overrides: *content
---

<p>You can override the <xref href="System.Web.UI.Design.WebControls.LoginNameDesigner.UsePreviewControl"></xref> property to return `false` or to determine its value based on whether the control is marked with a class level <xref href="System.Web.UI.Design.SupportsPreviewControlAttribute"></xref> object. If the actual <xref href="System.Web.UI.WebControls.LoginName"></xref> control is used to generate the design time markup, the control may not be visible on the design surface, since the runtime behavior of the control is to not render if the user identity is not known.</p>


