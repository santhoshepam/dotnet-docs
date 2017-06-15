---
summary: Creates a new <xref href="System.Xml.Linq.XDocument"></xref> from a string, optionally preserving white space, setting the base URI, and retaining line information.
remarks: This method parses a string and creates an XML tree.
example:
- "The following example creates a string that contains XML. It then parses the string into an <xref:System.Xml.Linq.XDocument>.  \n  \n```csharp  \n  \n                string str =  \n@\"<?xml version=\"\"1.0\"\"?>  \n<!-- comment at the root level -->  \n<Root>  \n    <Child>Content</Child>  \n</Root>\";  \nXDocument doc = XDocument.Parse(str);  \nConsole.WriteLine(doc);  \n```  \n  \n```vb  \n  \n                Dim str As String = _  \n    \"<?xml version= '1.0'?>\" & _  \n    \"<!-- comment at the root level -->\" & _  \n    \"<Root>\" & _  \n    \"  <Child>Content</Child>\" & _  \n    \"</Root>\"  \n  \nDim doc As XDocument = XDocument.Parse(str)  \nConsole.WriteLine(doc)  \n  \n```  \n  \n This example produces the following output:  \n  \n```xml  \n  \n                <!-- comment at the root level -->  \n<Root>  \n  <Child>Content</Child>  \n</Root>  \n```"
uid: System.Xml.Linq.XDocument.Parse*
---
