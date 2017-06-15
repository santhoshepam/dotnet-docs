---
uid: System.Web.UI.Design.IHierarchicalDataSourceDesigner.SuppressDataSourceEvents
additional_notes.overrides: *content
---

<p>Typically, you would call the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.SuppressDataSourceEvents"></xref> method when opening a dialog box, such as with the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.Configure"></xref> method, or during a call to the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.RefreshSchema(System.Boolean)"></xref> method, if building the schema requires multiple processes, any of which might create an exception. After processing is finished, call the <xref href="System.Web.UI.Design.IHierarchicalDataSourceDesigner.ResumeDataSourceEvents"></xref> method.</p>


