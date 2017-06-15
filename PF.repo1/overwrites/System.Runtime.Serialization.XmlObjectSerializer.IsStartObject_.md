---
summary: Gets a value that specifies whether the serializer can read the object.
remarks: "This method checks whether the reader is positioned on an element to read, and returns `true` if the element is the top-level element for the object found in the XML stream or document. To return `true`, the found element must have an expected name. The actual expected element name depends on the implementation of the serializer.  \n  \n With the <xref:System.Runtime.Serialization.DataContractSerializer>, the starting element is specified in the constructor of the extension class.  For an example, see the constructors for the <xref:System.Runtime.Serialization.DataContractSerializer> class."
uid: System.Runtime.Serialization.XmlObjectSerializer.IsStartObject*
---
