---
uid: System.Web.UI.HtmlTextWriter.OnAttributeRender(System.String,System.String,System.Web.UI.HtmlTextWriterAttribute)
additional_notes.overrides: *content
---

<p>If you inherit from the <xref href="System.Web.UI.HtmlTextWriter"></xref> class, you can override the <xref href="System.Web.UI.HtmlTextWriter.OnAttributeRender(System.String,System.String,System.Web.UI.HtmlTextWriterAttribute)"></xref> method to return `false` to prevent an attribute from being rendered at all, being rendered on a particular element, or being rendered for a particular markup. For example, if you do not want the object derived from <xref href="System.Web.UI.HtmlTextWriter"></xref> to render the `bgcolor` attribute to `<table>` elements, you can override the <xref href="System.Web.UI.HtmlTextWriter.OnAttributeRender(System.String,System.String,System.Web.UI.HtmlTextWriterAttribute)"></xref> and return `false` when <code>name</code> passes `bgcolor` and the <xref href="System.Web.UI.HtmlTextWriter.TagName"></xref> property value is `table`.</p>


