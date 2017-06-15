---
uid: System.Web.Script.Serialization.JavaScriptConverter
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.Web.Script.Serialization.JavaScriptConverter"></xref>, you must override the following members:  
  
-   <xref href="System.Web.Script.Serialization.JavaScriptConverter.Deserialize(System.Collections.Generic.IDictionary{System.String,System.Object},System.Type,System.Web.Script.Serialization.JavaScriptSerializer)"></xref>  
  
-   <xref href="System.Web.Script.Serialization.JavaScriptConverter.Serialize(System.Object,System.Web.Script.Serialization.JavaScriptSerializer)"></xref>  
  
-   <xref href="System.Web.Script.Serialization.JavaScriptConverter.SupportedTypes"></xref><xref href="System.Web.Script.Serialization.JavaScriptSerializer"></xref> provides the <xref href="System.Web.Script.Serialization.JavaScriptSerializer.ConvertToType``1(System.Object)"></xref> method that will be used by implementers of <xref href="System.Web.Script.Serialization.JavaScriptConverter"></xref>. Converter code must be able to take a value that is contained in the dictionary that the serializer passes to it, and then convert that value into an object of type <code>T</code>. Rather than re-implementing the custom conversion code to accomplish this, you can call the <xref href="System.Web.Script.Serialization.JavaScriptSerializer.ConvertToType``1(System.Object)"></xref> method.</p>


