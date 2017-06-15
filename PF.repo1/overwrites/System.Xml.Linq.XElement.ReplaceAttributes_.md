---
summary: Replaces the attributes of this element with the specified content.
remarks: "This method will raise the <xref:System.Xml.Linq.XObject.Changed> and the <xref:System.Xml.Linq.XObject.Changing> events.  \n  \n For details about the valid content that can be passed to this function, see [Valid Content of XElement and XDocument Objects](http://msdn.microsoft.com/library/aee2d319-5c5f-4b99-9bb4-2f58232577ae)."
example:
- "The following example creates an element with three attributes. It then uses this method to replace all of the attributes of the element with a single attribute.  \n  \n```csharp  \n  \n                XElement root = new XElement(\"Root\",  \n    new XAttribute(\"Att1\", 1),  \n    new XAttribute(\"Att2\", 2),  \n    new XAttribute(\"Att3\", 3)  \n);  \nroot.ReplaceAttributes(  \n    new XAttribute(\"NewAtt1\", 101)  \n);  \nConsole.WriteLine(root);  \n```  \n  \n```vb  \n  \n                Dim root As XElement = <Root Att1=\"1\" Att2=\"2\" Att3=\"3\"/>  \nroot.ReplaceAttributes(New XAttribute(\"NewAtt1\", 101))  \nConsole.WriteLine(root)  \n```  \n  \n This example produces the following output:  \n  \n```xml  \n  \n<Root NewAtt1=\"101\" />  \n```"
uid: System.Xml.Linq.XElement.ReplaceAttributes*
---
