---
uid: System.Web.UI.Design.ControlDesigner.UsePreviewControl
additional_notes.overrides: *content
---

<p>Custom designers that are derived from the <xref href="System.Web.UI.Design.ControlDesigner"></xref> class can override the <xref href="System.Web.UI.Design.ControlDesigner.UsePreviewControl"></xref> property and ignore the <xref href="System.Web.UI.Design.SupportsPreviewControlAttribute"></xref> object. Generally, to indicate that the <xref href="System.Web.UI.Design.ControlDesigner.ViewControl"></xref> property always returns a temporary copy of the control, override the <xref href="System.Web.UI.Design.ControlDesigner.UsePreviewControl"></xref> property to always return `true`. To indicate that the <xref href="System.Web.UI.Design.ControlDesigner.ViewControl"></xref> property always returns an instance of the control, override the <xref href="System.Web.UI.Design.ControlDesigner.UsePreviewControl"></xref> property to always return `false`. For example, the <xref href="System.Web.UI.Design.WebControls.PreviewControlDesigner"></xref> class derives from the <xref href="System.Web.UI.Design.ControlDesigner"></xref> and always returns `true` for the <xref href="System.Web.UI.Design.ControlDesigner.UsePreviewControl"></xref> property.</p>


