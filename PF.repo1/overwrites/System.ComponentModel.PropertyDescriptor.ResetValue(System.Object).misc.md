---
uid: System.ComponentModel.PropertyDescriptor.ResetValue(System.Object)
additional_notes.overrides: *content
---

<p>When overridden in a derived class, this method looks for a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>. If it finds one, it sets the value of the property to the <xref href="System.ComponentModel.DefaultValueAttribute"></xref> it found. If this method cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>, it looks for a "ResetMyProperty" method that you need to implement. If this is found, the <xref href="System.ComponentModel.PropertyDescriptor.ResetValue(System.Object)"></xref> method invokes it. If <xref href="System.ComponentModel.PropertyDescriptor.ResetValue(System.Object)"></xref> cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref> or a "ResetMyProperty" method that you implemented, it does not perform an operation.</p>


