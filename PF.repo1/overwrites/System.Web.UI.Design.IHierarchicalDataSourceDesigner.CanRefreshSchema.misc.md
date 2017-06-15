---
uid: System.Web.UI.Design.IHierarchicalDataSourceDesigner.CanRefreshSchema
additional_notes.overrides: *content
---

<p>If you implement the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner"></xref> interface to create your own data source and the schema will never change, the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.CanRefreshSchema"></xref> property should always return `false` and the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.RefreshSchema(System.Boolean)"></xref> method should raise a <xref href="System.NotSupportedException"></xref>.</p>


