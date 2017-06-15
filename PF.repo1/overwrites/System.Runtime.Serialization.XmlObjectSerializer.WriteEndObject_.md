---
summary: Writes the closing XML element to an XML stream or document.
remarks: 'The <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteStartObject%2A>, <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteObjectContent%2A>, and <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteEndObject%2A> methods must be implemented. The three methods are used in succession to write the complete serialization using the pattern: write start, write content, and write end. Users can insert XML attributes during the writing of the object between the calls to <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteStartObject%2A> and <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteEndObject%2A>. The three methods are also called by the virtual implementation of the <xref:System.Runtime.Serialization.XmlObjectSerializer.WriteObject%2A> method.'
uid: System.Runtime.Serialization.XmlObjectSerializer.WriteEndObject*
---
