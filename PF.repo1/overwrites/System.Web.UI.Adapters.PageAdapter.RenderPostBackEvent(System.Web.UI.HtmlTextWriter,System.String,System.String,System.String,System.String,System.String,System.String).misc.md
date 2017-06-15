---
uid: System.Web.UI.Adapters.PageAdapter.RenderPostBackEvent(System.Web.UI.HtmlTextWriter,System.String,System.String,System.String,System.String,System.String,System.String)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.PageAdapter"></xref> class, you can override the <xref href="System.Web.UI.Adapters.PageAdapter.RenderPostBackEvent(System.Web.UI.HtmlTextWriter,System.String,System.String,System.String,System.String,System.String,System.String)"></xref> method if a different format is required for the postback event hyperlink or the browser has other unique requirements. For example, some browsers require the hyperlink text to be nonempty if the link is to render. You can also override <xref href="System.Web.UI.Adapters.PageAdapter.RenderPostBackEvent(System.Web.UI.HtmlTextWriter,System.String,System.String,System.String,System.String,System.String,System.String)"></xref> if limited resources prevent including the view state as a URL parameter. The <xref href="System.Web.UI.Adapters.PageAdapter.RenderPostBackEvent(System.Web.UI.HtmlTextWriter,System.String,System.String,System.String,System.String,System.String,System.String)"></xref> base method does not write an attribute for <code>softkeyLabel</code>.</p>


