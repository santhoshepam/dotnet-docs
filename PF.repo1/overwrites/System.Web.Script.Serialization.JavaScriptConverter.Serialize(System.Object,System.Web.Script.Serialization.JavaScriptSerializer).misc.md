---
uid: System.Web.Script.Serialization.JavaScriptConverter.Serialize(System.Object,System.Web.Script.Serialization.JavaScriptSerializer)
additional_notes.overrides: *content
---

<p>The return value of <xref href="System.Web.Script.Serialization.JavaScriptConverter.Serialize(System.Object,System.Web.Script.Serialization.JavaScriptSerializer)"></xref> must be an <xref href="System.Collections.Generic.IDictionary`2"></xref> instance with zero or more name/value pairs that represent an object’s data to be converted to JSON. The converter itself does not serialize data as JSON. Instead, the converter builds a dictionary of name/value pairs that contain the property names (the string key for the dictionary) and corresponding property values (the object value in the dictionary). The <xref href="System.Web.Script.Serialization.JavaScriptSerializer"></xref> instance subsequently converts these to JSON.  
  
 If the converter encounters an exception, it should throw an <xref href="System.InvalidOperationException"></xref> error that describes the problem.</p>


