---
uid: System.ComponentModel.PropertyDescriptor.CanResetValue(System.Object)
additional_notes.overrides: *content
---

<p>When overridden in a derived class, this method looks for a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>. If it finds one, it compares the value of the attribute with the property's current value. It returns `true` when the default value does not match the property's current value. If this method cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>, it looks for a "ShouldPersistMyProperty" method that you need to implement yourself. If this is found, <xref href="System.ComponentModel.PropertyDescriptor.CanResetValue(System.Object)"></xref> returns what "ShouldPersistMyProperty" returns. Otherwise, it looks for a "ResetMyProperty" method that you need to implement yourself. If this is found, <xref href="System.ComponentModel.PropertyDescriptor.CanResetValue(System.Object)"></xref> returns `true`. If it cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>, a "ShouldPersistMyProperty" method, or a "ResetMyProperty" method, then it returns `false`.</p>


