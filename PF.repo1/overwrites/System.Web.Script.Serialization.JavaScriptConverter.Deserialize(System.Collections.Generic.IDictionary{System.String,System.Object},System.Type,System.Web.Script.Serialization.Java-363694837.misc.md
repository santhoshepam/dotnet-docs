---
uid: System.Web.Script.Serialization.JavaScriptConverter.Deserialize(System.Collections.Generic.IDictionary{System.String,System.Object},System.Type,System.Web.Script.Serialization.JavaScriptSerializer)
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.Script.Serialization.JavaScriptConverter.Deserialize(System.Collections.Generic.IDictionary{System.String,System.Object},System.Type,System.Web.Script.Serialization.JavaScriptSerializer)"></xref> method iterates through the values in the <code>dictionary</code> parameter to construct an instance of the type requested in the <code>type</code> parameter. Although a converter can directly use values from <code>dictionary</code>, we recommend that the converter implementer use the <xref href="System.Web.Script.Serialization.JavaScriptSerializer.ConvertToType``1(System.Object)"></xref> method instead. The converter should call this method of the <xref href="System.Web.Script.Serialization.JavaScriptSerializer"></xref> instance available from the <code>serializer</code> parameter.  
  
 The <xref href="System.Web.Script.Serialization.JavaScriptSerializer.ConvertToType``1(System.Object)"></xref> method enables converter to pass a property value from <code>dictionary</code>, and then return a value of the expected type. In some cases, a converter for a custom type might be working with properties that themselves have registered converters (for example, type A has a property of type B, and type B is also associated with a custom converter). In that case, invoking <xref href="System.Web.Script.Serialization.JavaScriptSerializer.ConvertToType``1(System.Object)"></xref> makes sure that custom converters will be recursively invoked for property data that is contained in the dictionary. When the converter has iterated through all entries in the dictionary, it returns a constructed instance of the target type.  
  
 If the converter encounters a problem during deserialization, it should throw an <xref href="System.InvalidOperationException"></xref> error that describes the problem.</p>


