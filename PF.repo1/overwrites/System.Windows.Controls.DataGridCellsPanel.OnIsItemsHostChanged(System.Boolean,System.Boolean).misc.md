---
uid: System.Windows.Controls.DataGridCellsPanel.OnIsItemsHostChanged(System.Boolean,System.Boolean)
additional_notes.overrides: *content
---

<p>You can override this method and use it as a notification that the <xref href="System.Windows.Controls.Panel.IsItemsHost"></xref> property has changed. Then perform your own logic based on the old and new values. Be sure to call the base class’s <xref href="System.Windows.Controls.DataGridCellsPanel.OnIsItemsHostChanged(System.Boolean,System.Boolean)"></xref> method; otherwise, important functionality will be disabled. The base implementation synchronizes the <xref href="System.Windows.Controls.DataGridCellsPanel"></xref> with the <xref href="System.Windows.Controls.Primitives.DataGridCellsPresenter"></xref> or <xref href="System.Windows.Controls.Primitives.DataGridColumnHeadersPresenter"></xref> that it is associated with.</p>


