---
uid: System.Web.UI.Design.ControlDesigner.GetErrorDesignTimeHtml(System.Exception)
additional_notes.overrides: *content
---

<p>The typical design pattern is to try to get HTML markup through the associated control, and then if an error is encountered, call the <xref href="System.Web.UI.Design.ControlDesigner.GetErrorDesignTimeHtml(System.Exception)"></xref> method. If no markup is returned by the control, call the <xref href="System.Web.UI.Design.ControlDesigner.GetEmptyDesignTimeHtml"></xref> method, which if it is not overridden to provide specific markup, calls the <xref href="System.Web.UI.Design.ControlDesigner.CreatePlaceHolderDesignTimeHtml"></xref> method, which should contain information about the type and ID of the control.</p>


