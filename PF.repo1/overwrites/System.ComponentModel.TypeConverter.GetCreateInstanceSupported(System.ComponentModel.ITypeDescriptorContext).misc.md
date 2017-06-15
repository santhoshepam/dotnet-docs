---
uid: System.ComponentModel.TypeConverter.GetCreateInstanceSupported(System.ComponentModel.ITypeDescriptorContext)
additional_notes.overrides: *content
---

<p>Override this method if the type you want to convert must re-create the object to change its value.  
  
 Use the <code>context</code> parameter to extract additional information about the environment from which this converter is invoked. This parameter can be `null`, so always check it. Also, properties on the context object can return `null`.</p>


