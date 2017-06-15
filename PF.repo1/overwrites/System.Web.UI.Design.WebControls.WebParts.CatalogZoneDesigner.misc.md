---
uid: System.Web.UI.Design.WebControls.WebParts.CatalogZoneDesigner
additional_notes.overrides: *content
---

<p>If you want to override the <xref href="System.Web.UI.Design.WebControls.WebParts.CatalogZoneDesigner.GetDesignTimeHtml"></xref> method to change the design-time appearance of your custom control, make sure to use the <xref href="System.Web.UI.Design.WebControls.WebParts.CatalogZoneDesigner.GetDesignTimeHtml(System.Web.UI.Design.DesignerRegionCollection)"></xref> method and invoke the parent method before adding custom code, because that is the method that creates the rendering for the regions in the control. If you override <xref href="System.Web.UI.Design.WebControls.WebParts.CatalogZoneDesigner.GetDesignTimeHtml"></xref> and do not call <xref href="System.Web.UI.Design.WebControls.WebParts.CatalogZoneDesigner.GetDesignTimeHtml(System.Web.UI.Design.DesignerRegionCollection)"></xref> somewhere in the method, your designer regions will not be rendered.</p>


