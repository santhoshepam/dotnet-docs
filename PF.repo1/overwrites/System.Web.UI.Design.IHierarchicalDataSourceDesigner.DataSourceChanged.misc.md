---
uid: System.Web.UI.Design.IHierarchicalDataSourceDesigner.DataSourceChanged
additional_notes.overrides: *content
---

<p>Typically, when you implement the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner"></xref> interface, the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.DataSourceChanged"></xref> event handler calls the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.RefreshSchema(System.Boolean)"></xref> method. If the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.CanRefreshSchema"></xref> property is `true`, recreate any sample data, and then raise the event again to allow each data-bound control to refresh its markup.</p>


