---
uid: System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderBeginTag(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderBeginTag(System.Web.UI.HtmlTextWriter)"></xref> base method calls the <xref href="System.Web.UI.WebControls.WebControl.RenderBeginTag(System.Web.UI.HtmlTextWriter)"></xref> method. In turn, the <xref href="System.Web.UI.WebControls.WebControl.RenderBeginTag(System.Web.UI.HtmlTextWriter)"></xref> base method calls the appropriate <xref href="System.Web.UI.HtmlTextWriter.RenderBeginTag(System.Web.UI.HtmlTextWriterTag)"></xref> overload, which is determined by the type of tag with which the <xref href="System.Web.UI.WebControls.WebControl"></xref> object was created. You can avoid overriding <xref href="System.Web.UI.WebControls.Adapters.WebControlAdapter.RenderBeginTag(System.Web.UI.HtmlTextWriter)"></xref> by deriving from the <xref href="System.Web.UI.HtmlTextWriter"></xref> class and overriding <xref href="System.Web.UI.HtmlTextWriter.RenderBeginTag(System.Web.UI.HtmlTextWriterTag)"></xref>, and also possibly <xref href="System.Web.UI.HtmlTextWriter.RenderEndTag"></xref>.</p>


