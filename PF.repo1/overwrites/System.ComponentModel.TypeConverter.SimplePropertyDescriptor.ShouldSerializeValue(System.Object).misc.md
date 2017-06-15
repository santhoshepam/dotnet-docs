---
uid: System.ComponentModel.TypeConverter.SimplePropertyDescriptor.ShouldSerializeValue(System.Object)
additional_notes.overrides: *content
---

<p>When overridden in a derived class, this method returns `true` if the current value of the property is different from its default value. It looks for a default value by first looking for a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>. If the method finds this attribute, it compares the value of the attribute with the current value of the property. If this method cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>, it looks for a <code>ShouldSerializeMyProperty</code> method. If this method finds a <code>ShouldSerializeMyProperty</code> method, it invokes it. If this method cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref> or a <code>ShouldSerializeMyProperty</code> method, it cannot create optimizations and it returns `true`.</p>


