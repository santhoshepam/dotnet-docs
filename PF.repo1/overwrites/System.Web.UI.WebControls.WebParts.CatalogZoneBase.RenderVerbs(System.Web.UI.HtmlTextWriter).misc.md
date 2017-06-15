---
uid: System.Web.UI.WebControls.WebParts.CatalogZoneBase.RenderVerbs(System.Web.UI.HtmlTextWriter)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase.RenderVerbs(System.Web.UI.HtmlTextWriter)"></xref> method does not handle the rendering for any custom <xref href="System.Web.UI.WebControls.WebParts.WebPartVerb"></xref> objects that a developer adds to a custom <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase"></xref> zone. If you want to add custom verbs to a <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase"></xref> class, you must inherit from the <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase"></xref> class, and override the <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase.RenderVerbs(System.Web.UI.HtmlTextWriter)"></xref> method, which you can use to render the custom verbs for your zone. You must also override the <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase.RaisePostBackEvent(System.String)"></xref> method to handle the event when a custom verb is clicked by a user.</p>


