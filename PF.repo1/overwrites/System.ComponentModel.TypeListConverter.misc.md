---
uid: System.ComponentModel.TypeListConverter
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.ComponentModel.TypeListConverter"></xref>, you can override the following methods.  
  
-   To support custom type conversion, override the <xref href="System.ComponentModel.TypeConverter.CanConvertFrom(System.Type)"></xref>, <xref href="System.ComponentModel.TypeConverter.CanConvertTo(System.Type)"></xref>, <xref href="System.ComponentModel.TypeConverter.ConvertFrom(System.Object)"></xref>, and <xref href="System.ComponentModel.TypeConverter.ConvertTo(System.Object,System.Type)"></xref> methods.  
  
-   To convert types that must re-create the object to change its value, override the <xref href="System.ComponentModel.TypeConverter.CreateInstance(System.Collections.IDictionary)"></xref> and <xref href="System.ComponentModel.TypeConverter.GetCreateInstanceSupported"></xref> methods.  
  
-   To convert types that support properties, override the <xref href="System.ComponentModel.TypeConverter.GetProperties(System.Object)"></xref> and <xref href="System.ComponentModel.TypeConverter.GetPropertiesSupported"></xref> methods. If the class you are converting does not have properties, and you need to implement properties, you can use the <xref href="System.ComponentModel.TypeConverter.SimplePropertyDescriptor"></xref> class as a base for implementing the property descriptors. When you inherit from <xref href="System.ComponentModel.TypeConverter.SimplePropertyDescriptor"></xref>, you must override the <xref href="System.ComponentModel.PropertyDescriptor.GetValue(System.Object)"></xref> and <xref href="System.ComponentModel.PropertyDescriptor.SetValue(System.Object,System.Object)"></xref> methods.  
  
-   To convert types that support standard values, override the <xref href="System.ComponentModel.TypeConverter.GetStandardValues"></xref>, <xref href="System.ComponentModel.TypeConverter.GetStandardValuesExclusive"></xref>, <xref href="System.ComponentModel.TypeConverter.GetStandardValuesSupported"></xref> and <xref href="System.ComponentModel.TypeConverter.IsValid(System.Object)"></xref> methods.</p>


