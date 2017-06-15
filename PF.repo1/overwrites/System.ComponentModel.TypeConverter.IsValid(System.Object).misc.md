---
uid: System.ComponentModel.TypeConverter.IsValid(System.Object)
additional_notes.overrides: *content
---

<p>Override this method if the type you want to convert supports standard values that can be validated.  
  
 The <xref href="System.ComponentModel.TypeConverter.IsValid(System.Object)"></xref> method is used to validate a value within the type rather than to determine if <code>value</code> can be converted to the given type. For example, <xref href="System.ComponentModel.TypeConverter.IsValid(System.Object)"></xref> can be used to determine if a given value is valid for an enumeration type. For an example, see <xref href="System.ComponentModel.EnumConverter"></xref>.  
  
 You can write your own <code>WillConvertSucceed</code> method by wrapping the <xref href="System.ComponentModel.TypeConverter.ConvertTo*"></xref> and <xref href="System.ComponentModel.TypeConverter.ConvertFrom*"></xref> methods in exception blocks.</p>


