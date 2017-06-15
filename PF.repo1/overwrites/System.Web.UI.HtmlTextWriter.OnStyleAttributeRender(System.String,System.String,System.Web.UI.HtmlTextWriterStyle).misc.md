---
uid: System.Web.UI.HtmlTextWriter.OnStyleAttributeRender(System.String,System.String,System.Web.UI.HtmlTextWriterStyle)
additional_notes.overrides: *content
---

<p>If you inherit from the <xref href="System.Web.UI.HtmlTextWriter"></xref> class, you can override the <xref href="System.Web.UI.HtmlTextWriter.OnStyleAttributeRender(System.String,System.String,System.Web.UI.HtmlTextWriterStyle)"></xref> method to return `false` to prevent a style attribute from being rendered at all, being rendered on a particular element, or being rendered for a particular markup language. For example, if you do not want the object that is derived from <xref href="System.Web.UI.HtmlTextWriter"></xref> to render the `color` style attribute to a `<p>` element, you can override the <xref href="System.Web.UI.HtmlTextWriter.OnStyleAttributeRender(System.String,System.String,System.Web.UI.HtmlTextWriterStyle)"></xref> and return `false` when <code>name</code> passes `color` and the <xref href="System.Web.UI.HtmlTextWriter.TagName"></xref> property value is `p`.</p>


