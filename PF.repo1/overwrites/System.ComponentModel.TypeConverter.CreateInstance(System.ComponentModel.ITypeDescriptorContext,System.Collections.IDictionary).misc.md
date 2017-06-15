---
uid: System.ComponentModel.TypeConverter.CreateInstance(System.ComponentModel.ITypeDescriptorContext,System.Collections.IDictionary)
additional_notes.overrides: *content
---

<p>Override this method if the type you want to convert must re-create the object to change its value.  
  
 Use the <code>context</code> parameter to extract additional information about the environment from which this converter is invoked. This parameter can be `null`, so always check it. Also, properties on the context object can return `null`.  
  
 The dictionary provided by the <code>propertyValues</code> parameter has a series of name/value pairs, one for each property returned from <xref href="System.ComponentModel.TypeConverter.GetProperties(System.Object)"></xref>.</p>


