---
uid: System.Web.UI.WebControls.BaseDataBoundControl.ValidateDataSource(System.Object)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.WebControls.BaseDataBoundControl.ValidateDataSource(System.Object)"></xref> method is only called in the <xref href="System.Web.UI.WebControls.BaseDataBoundControl"></xref> class's mutator (setter) for the <xref href="System.Web.UI.WebControls.BaseDataBoundControl.DataSource"></xref> property. Derived classes implement the method to check the type of the object that is set for the <xref href="System.Web.UI.WebControls.BaseDataBoundControl.DataSource"></xref> property, to ensure that the data-bound control can work with the type. If the type is not recognized, derived type implementations throw an exception.</p>


