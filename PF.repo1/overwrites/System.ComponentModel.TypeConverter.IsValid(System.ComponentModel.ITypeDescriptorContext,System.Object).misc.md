---
uid: System.ComponentModel.TypeConverter.IsValid(System.ComponentModel.ITypeDescriptorContext,System.Object)
additional_notes.overrides: *content
---

<p>Override this method if the type you want to convert supports standard values that can be validated.  
  
 The <xref href="System.ComponentModel.TypeConverter.IsValid(System.ComponentModel.ITypeDescriptorContext,System.Object)"></xref> method is used to validate a value within the type rather than to determine if <code>value</code> can be converted to the given type. For example, <xref href="System.ComponentModel.TypeConverter.IsValid(System.ComponentModel.ITypeDescriptorContext,System.Object)"></xref> can be used to determine if a given value is valid for an enumeration type. For an example, see <xref href="System.ComponentModel.EnumConverter"></xref>.</p>


