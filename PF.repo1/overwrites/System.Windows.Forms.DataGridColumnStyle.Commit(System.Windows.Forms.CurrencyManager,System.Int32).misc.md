---
uid: System.Windows.Forms.DataGridColumnStyle.Commit(System.Windows.Forms.CurrencyManager,System.Int32)
additional_notes.overrides: *content
---

<p>The <xref href="System.Windows.Forms.DataGridColumnStyle.Commit(System.Windows.Forms.CurrencyManager,System.Int32)"></xref> method should be used by classes derived from the <xref href="System.Windows.Forms.DataGridColumnStyle"></xref> class to reset their editing state, for example, to concede the focus if the <xref href="System.Windows.Forms.DataGridColumnStyle"></xref> hosts an editing control. See the <xref href="System.Windows.Forms.DataGridColumnStyle.ConcedeFocus"></xref> method.  
  
 Call the <xref href="System.Windows.Forms.DataGridColumnStyle.Commit(System.Windows.Forms.CurrencyManager,System.Int32)"></xref> method when the <xref href="System.Windows.Forms.DataGridColumnStyle"></xref> receives a request to complete editing. If this is not possible without error, return `false`.  
  
 The <xref href="System.Windows.Forms.DataGridColumnStyle.Commit(System.Windows.Forms.CurrencyManager,System.Int32)"></xref> method is called by the public method <xref href="System.Windows.Forms.DataGrid.OnMouseDown(System.Windows.Forms.MouseEventArgs)"></xref> of the <xref href="System.Windows.Forms.DataGrid"></xref> control. The method is also called by other private methods, for example, when the current row is changed.</p>


