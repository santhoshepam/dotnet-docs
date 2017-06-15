---
uid: System.Web.UI.Design.IHierarchicalDataSourceDesigner.RefreshSchema(System.Boolean)
additional_notes.overrides: *content
---

<p>If you implement the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner"></xref> interface to create your own data source and the schema will never change, the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.CanRefreshSchema"></xref> property should always return `false` and the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.RefreshSchema(System.Boolean)"></xref> method should raise a <xref href="System.NotSupportedException"></xref>.  
  
 Typically, if the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.RefreshSchema(System.Boolean)"></xref> is called by the design host as a result of user action, the <code>preferSilent</code> parameter would be `false`, because the user would expect to be notified of any problems with refreshing the schema. But, if the schema is refreshed implicitly, such as after a call to the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.Configure"></xref> method, or if the refreshing process involves a number of steps, <code>preferSilent</code> should be set to `true`.</p>


