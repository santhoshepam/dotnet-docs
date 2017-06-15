---
uid: System.Web.UI.Design.WebControls.DataSourceIDConverter.IsValidDataSource(System.ComponentModel.IComponent)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.Design.WebControls.DataSourceIDConverter.IsValidDataSource(System.ComponentModel.IComponent)"></xref> method should be overridden by controls that need to further investigate a given component to decide whether it should be returned in the list of standard values. For example, if a control works with only <xref href="System.Web.UI.WebControls.XmlDataSource"></xref> data sources, <xref href="System.Web.UI.Design.WebControls.DataSourceIDConverter.IsValidDataSource(System.ComponentModel.IComponent)"></xref> should return `true` only for those components that are <xref href="System.Web.UI.WebControls.XmlDataSource"></xref> objects.</p>


