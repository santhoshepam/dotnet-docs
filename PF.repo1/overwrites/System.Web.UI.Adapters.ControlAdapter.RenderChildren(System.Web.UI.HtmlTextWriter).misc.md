---
uid: System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.ControlAdapter"></xref> class, for a composite control, the adapter developer must ensure that the child controls are rendered. If the adapter overrides the <xref href="System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> method, it should call the <xref href="System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> method from an override of the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> method.  
  
 If the <xref href="System.Web.UI.Control.Render(System.Web.UI.HtmlTextWriter)"></xref> method causes the child controls to be rendered but itself does not generate markup, it might be appropriate for the <xref href="System.Web.UI.Adapters.ControlAdapter.Render(System.Web.UI.HtmlTextWriter)"></xref> method to call its base method, which calls the <xref href="System.Web.UI.Control.Render(System.Web.UI.HtmlTextWriter)"></xref> method, instead of implementing an override for the <xref href="System.Web.UI.Adapters.ControlAdapter.RenderChildren(System.Web.UI.HtmlTextWriter)"></xref> method.</p>


