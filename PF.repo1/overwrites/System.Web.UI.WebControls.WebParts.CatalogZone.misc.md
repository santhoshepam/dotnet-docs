---
uid: System.Web.UI.WebControls.WebParts.CatalogZone
additional_notes.overrides: *content
---

<p>You can create custom <xref href="System.Web.UI.WebControls.WebParts.CatalogZone"></xref> classes if you want more control over the rendering and behavior of the catalog UI. If you do not need to provide users of your control with the ability to add <xref href="System.Web.UI.WebControls.WebParts.CatalogPart"></xref> controls declaratively, then you can inherit directly from the <xref href="System.Web.UI.WebControls.WebParts.CatalogZoneBase"></xref> class. If you do want to enable controls to be added declaratively, the simples approach is to inherit from the <xref href="System.Web.UI.WebControls.WebParts.CatalogZone"></xref> class, because it provides the essential zone template.  
  
 If you inherit from the <xref href="System.Web.UI.WebControls.WebParts.CatalogZone"></xref> class, you can override the <xref href="System.Web.UI.WebControls.WebParts.CatalogZone.CreateCatalogParts"></xref> method and use the method to add custom <xref href="System.Web.UI.WebControls.WebParts.CatalogPart"></xref> controls to a <xref href="System.Web.UI.WebControls.WebParts.CatalogPartCollection"></xref>, if you want greater programmatic control over adding custom <xref href="System.Web.UI.WebControls.WebParts.CatalogPart"></xref> controls to your zone.</p>


