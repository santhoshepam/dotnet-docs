---
summary: Creates an instance of <xref href="System.Xml.XmlDictionaryWriter"></xref> that writes [!INCLUDE[indigo2](~/includes/indigo2-md.md)] binary XML format.
remarks: "The binary format only supports one text node as the attribute value and therefore buffers the values written to it to emit a single node, as shown in the following sample code.  \n  \n```  \nXmlWriter binarywriter = XmlDictionaryWriter.CreateBinaryWriter(Stream.Null);  \nbinarywriter.WriteStartAttribute(\"StartAttribute\");  \nstring largeStr = new string('r', 100000);  \nfor (int i = 0; i < 10000; i++)   \n{  \n    binarywriter.WriteValue(largeStr);  \n}  \nbinarywriter.WriteEndAttribute();  \n  \n```  \n  \n In the previous sample the code buffers about 1 GB of memory, while in the other writers it writes the values as they are provided."
uid: System.Xml.XmlDictionaryWriter.CreateBinaryWriter*
---
