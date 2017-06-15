---
uid: System.Web.UI.WebControls.Menu.DataBind
additional_notes.overrides: *content
---

<p>Data-bound controls should override <xref href="System.Web.UI.WebControls.Menu.PerformDataBinding"></xref> instead of <xref href="System.Web.UI.WebControls.Menu.DataBind"></xref>. If <xref href="System.Web.UI.WebControls.Menu.DataBind"></xref> is overridden, the <xref href="System.Web.UI.WebControls.Menu.OnDataBinding(System.EventArgs)"></xref> and <xref href="System.Web.UI.WebControls.BaseDataBoundControl.OnDataBound(System.EventArgs)"></xref> events are raised in the wrong order.</p>


