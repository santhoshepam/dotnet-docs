---
uid: System.Windows.Forms.DataGridViewCell
additional_notes.overrides: *content
---

<p>When you derive from <xref href="System.Windows.Forms.DataGridViewCell"></xref> and add new properties to the derived class, be sure to override the <xref href="System.Windows.Forms.DataGridViewCell.Clone"></xref> method to copy the new properties during cloning operations. You should also call the base class's <xref href="System.Windows.Forms.DataGridViewCell.Clone"></xref> method so that the properties of the base class are copied to the new cell.</p>


