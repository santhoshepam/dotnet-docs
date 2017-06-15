---
uid: System.ComponentModel.PropertyDescriptor.ShouldSerializeValue(System.Object)
additional_notes.overrides: *content
---

<p>When overridden in a derived class, this method returns `true` if the current value of the property is different from its default value. It looks for a default value by first looking for a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>. If the method finds this attribute, it compares the value of the attribute with the property's current value. If this method cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref>, it looks for a "ShouldSerializeMyProperty" method that you need to implement. If it is found, <xref href="System.ComponentModel.PropertyDescriptor.ShouldSerializeValue(System.Object)"></xref> invokes it. If this method cannot find a <xref href="System.ComponentModel.DefaultValueAttribute"></xref> or a "ShouldSerializeMyProperty" method, it cannot create optimizations and it returns `true`.
 <block subset="none" type="note"><p>  
 The <xref href="System.ComponentModel.Design.ComponentDesigner"></xref> class implements special serialization logic for inherited components. For more information, see <xref href="System.ComponentModel.Design.ComponentDesigner"></xref>.  
</p></block></p>


