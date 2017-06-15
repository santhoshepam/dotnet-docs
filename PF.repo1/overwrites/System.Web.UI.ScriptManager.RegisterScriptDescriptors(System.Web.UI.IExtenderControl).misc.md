---
uid: System.Web.UI.ScriptManager.RegisterScriptDescriptors(System.Web.UI.IExtenderControl)
additional_notes.overrides: *content
---

<p>If you derive from the <xref href="System.Web.UI.ExtenderControl"></xref> class and override the <xref href="System.Web.UI.Control.Render(System.Web.UI.HtmlTextWriter)"></xref> method, but you do not call the base class method, you must call the <xref href="System.Web.UI.ScriptManager.RegisterScriptDescriptors(System.Web.UI.IExtenderControl)"></xref> method. This enables the <xref href="System.Web.UI.ScriptManager"></xref> control to render the instance scripts that support the client object that the control represents.</p>


