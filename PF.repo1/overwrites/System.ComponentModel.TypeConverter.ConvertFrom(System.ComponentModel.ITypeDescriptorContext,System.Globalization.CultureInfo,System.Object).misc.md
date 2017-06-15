---
uid: System.ComponentModel.TypeConverter.ConvertFrom(System.ComponentModel.ITypeDescriptorContext,System.Globalization.CultureInfo,System.Object)
additional_notes.overrides: *content
---

<p>Override this method to provide your own conversion requirements.  
  
 Use the <code>context</code> parameter to extract additional information about the environment from which this converter is invoked. This parameter can be `null`, so always check it. Also, properties on the context object can return `null`.  
  
 For implementation patterns for type converters that are used to support XAML and custom types, see [Type Converters for XAML Overview](~/docs/framework/xaml-services/type-converters-for-xaml-overview.md).</p>


