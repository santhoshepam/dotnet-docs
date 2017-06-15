---
uid: System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderContents(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>For a composite control, you must ensure that the child controls are rendered. If you override the <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderContents(System.Web.UI.HtmlTextWriter)"></xref> method and do not call its base method, you can cause the child controls to be rendered by calling <xref href="System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> which, if not overridden, calls <xref href="System.Web.UI.Control.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> from the <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderContents(System.Web.UI.HtmlTextWriter)"></xref> override.</p>


