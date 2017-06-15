---
uid: System.ComponentModel.TypeConverter.GetProperties(System.ComponentModel.ITypeDescriptorContext,System.Object,System.Attribute[])
additional_notes.overrides: *content
---

<p>Override this method if the type you want to convert supports properties.  
  
 Use the <code>context</code> parameter to extract additional information about the environment from which this converter is invoked. This parameter can be `null`, so always check it. Also, properties on the context object can return `null`.  
  
 The attributes array is used to filter the array. The attributes can have a mix of <xref href="System.Type"></xref> and <xref href="System.Attribute"></xref> objects. Filtering is defined by the following rules:  
  
-   A <xref href="System.Type"></xref> is treated as a wildcard; it matches a property that has the <xref href="System.Type"></xref> in its set of attributes.  
  
-   If a property does not have an <xref href="System.Attribute"></xref> of the same class, the property is not included in the returned array.  
  
-   If the attribute is an instance of <xref href="System.Attribute"></xref>, the property must be an exact match or it is not included in the returned array.  
  
-   If an <xref href="System.Attribute"></xref> instance is specified and it is the default property, it is included in the returned array even if there is no instance of the <xref href="System.Attribute"></xref> in the property.</p>


