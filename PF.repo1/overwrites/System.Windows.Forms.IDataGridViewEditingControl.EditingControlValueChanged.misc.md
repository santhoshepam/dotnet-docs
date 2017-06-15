---
uid: System.Windows.Forms.IDataGridViewEditingControl.EditingControlValueChanged
additional_notes.overrides: *content
---

<p>Returning `true` in your implementation of this property does not automatically change the displayed value. When the value changes in the editing control, you must notify the <xref href="System.Windows.Forms.DataGridView"></xref> of the change by passing `true` to the <xref href="System.Windows.Forms.DataGridView.NotifyCurrentCellDirty(System.Boolean)"></xref> method.</p>


