---
uid: System.Web.UI.WebControls.ControlIDConverter.FilterControl(System.Web.UI.Control)
additional_notes.overrides: *content
---

<p>The implementation of the <xref href="System.Web.UI.WebControls.ControlIDConverter.FilterControl(System.Web.UI.Control)"></xref> method returns `true` in all cases. Classes that derive from the <xref href="System.Web.UI.WebControls.ControlIDConverter"></xref> override this method to provide their own filtering mechanism. For example, the <xref href="System.Web.UI.WebControls.AssociatedControlConverter"></xref> class overrides the <xref href="System.Web.UI.WebControls.ControlIDConverter.FilterControl(System.Web.UI.Control)"></xref> method and returns `true` only if the control is a Web server control.</p>


