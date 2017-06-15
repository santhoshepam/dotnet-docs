---
uid: System.Web.UI.HtmlTextWriter.OnTagRender(System.String,System.Web.UI.HtmlTextWriterTag)
additional_notes.overrides: *content
---

<p>If you inherit from the <xref href="System.Web.UI.HtmlTextWriter"></xref> class, you can override the <xref href="System.Web.UI.HtmlTextWriter.OnTagRender(System.String,System.Web.UI.HtmlTextWriterTag)"></xref> method to return `false` to prevent a markup element from being rendered at all or for a particular markup language. For example, if you do not want the object that is derived from <xref href="System.Web.UI.HtmlTextWriter"></xref> to render the `<font>` element, you can override the <xref href="System.Web.UI.HtmlTextWriter.OnTagRender(System.String,System.Web.UI.HtmlTextWriterTag)"></xref> method to return `false` when a page is requested that contains a `<font>` element.</p>


