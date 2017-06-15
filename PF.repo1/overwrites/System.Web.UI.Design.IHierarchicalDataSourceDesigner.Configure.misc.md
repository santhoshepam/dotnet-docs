---
uid: System.Web.UI.Design.IHierarchicalDataSourceDesigner.Configure
additional_notes.overrides: *content
---

<p>If you implement the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner"></xref> interface to create your own data source and you do not provide configuration functionality, the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.CanConfigure"></xref> property should always return `false` and the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.Configure"></xref> method should raise a <xref href="System.NotSupportedException"></xref>.</p>


