---
uid: System.Windows.Forms.IDataGridViewEditingControl.GetEditingControlFormattedValue(System.Windows.Forms.DataGridViewDataErrorContexts)
additional_notes.overrides: *content
---

<p>Changing the return value in your implementation of this method does not automatically change the displayed value. When the value changes in the editing control, you must notify the <xref href="System.Windows.Forms.DataGridView"></xref> of the change by passing `true` to the <xref href="System.Windows.Forms.DataGridView.NotifyCurrentCellDirty(System.Boolean)"></xref> method.</p>


