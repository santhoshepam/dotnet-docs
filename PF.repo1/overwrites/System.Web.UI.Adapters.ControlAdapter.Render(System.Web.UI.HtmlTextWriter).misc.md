---
uid: System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.ControlAdapter"></xref> class, the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> base method calls the <xref href="System.Web.UI.Control.Render(System.Web.UI.HtmlTextWriter)"></xref> method. Thus, overrides of the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> method should call the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> base method only if its processing is in addition to, rather than instead of, the <xref href="System.Web.UI.Control.Render(System.Web.UI.HtmlTextWriter)"></xref> method.  
  
 For a composite control, the adapter developer must ensure that the child controls are rendered. If the <xref href="System.Web.UI.Control.Render(System.Web.UI.HtmlTextWriter)"></xref> method causes the child controls to be rendered but does not generate markup, it might be appropriate for the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> method to call its base method. If target-specific rendering of the child controls is necessary, the adapter should implement the <xref href="System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> method and call the <xref href="System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> method from the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> method.</p>


