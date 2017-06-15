---
uid: System.Web.UI.Adapters.ControlAdapter.EndRender(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.ControlAdapter"></xref> class, the <xref href="System.Web.UI.Adapters.ControlAdapter.EndRender(System.Web.UI.HtmlTextWriter)"></xref> base method calls the <xref href="System.Web.UI.HtmlTextWriter.EndRender"></xref> method. Thus, overrides of the <xref href="System.Web.UI.Adapters.ControlAdapter.EndRender(System.Web.UI.HtmlTextWriter)"></xref> method should call the <xref href="System.Web.UI.Adapters.ControlAdapter.EndRender(System.Web.UI.HtmlTextWriter)"></xref> base method only if its processing is in addition to, rather than instead of, the <xref href="System.Web.UI.HtmlTextWriter.EndRender"></xref> method.</p>


