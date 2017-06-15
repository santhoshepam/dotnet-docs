---
summary: Writes only the content of an object to an XML document or stream.
remarks: 'The <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteStartObject%2A>, <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteObjectContent%2A>, and <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteEndObject%2A> methods must be implemented. The three methods are used in succession to write the complete serialization using the pattern: write start, write content, and write end. If the implementation writes using XML elements, attributes can be inserted before writing the contents of the object. The three methods are also called by the virtual implementation of the <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteObject%2A> method.'
uid: System.Runtime.Serialization.XmlObjectSerializer.WriteObjectContent*
---
