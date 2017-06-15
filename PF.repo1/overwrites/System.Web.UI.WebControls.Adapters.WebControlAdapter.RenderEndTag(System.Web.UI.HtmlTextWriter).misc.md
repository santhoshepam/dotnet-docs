---
uid: System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderEndTag(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderEndTag(System.Web.UI.HtmlTextWriter)"></xref> base method calls the <xref href="System.Web.UI.WebControls.WebControl.RenderEndTag(System.Web.UI.HtmlTextWriter)"></xref> method. In turn, the <xref href="System.Web.UI.WebControls.WebControl.RenderEndTag(System.Web.UI.HtmlTextWriter)"></xref> base method calls the <xref href="System.Web.UI.HtmlTextWriter.RenderBeginTag(System.Web.UI.HtmlTextWriterTag)"></xref> method. You can avoid overriding <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderBeginTag(System.Web.UI.HtmlTextWriter)"></xref> by deriving from the <xref href="System.Web.UI.HtmlTextWriter"></xref> class and overriding <xref href="System.Web.UI.HtmlTextWriter.RenderEndTag"></xref>, and also possibly <xref href="System.Web.UI.HtmlTextWriter.RenderBeginTag(System.Web.UI.HtmlTextWriterTag)"></xref>.</p>


