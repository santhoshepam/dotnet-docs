---
uid: System.Web.UI.WebControls.Adapters.WebControlAdapter.Render(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> base method calls <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderBeginTag(System.Web.UI.HtmlTextWriter)"></xref>, then <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderContents(System.Web.UI.HtmlTextWriter)"></xref>, and then <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderEndTag(System.Web.UI.HtmlTextWriter)"></xref>. If you override <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> and do not call the base method, you must be sure to provide this functionality.</p>


