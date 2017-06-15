---
summary: Selects a list of nodes matching the XPath expression.
remarks: "XPath expressions can include namespaces. Namespace resolution is supported using the `XmlNamespaceManager`. If the XPath expression includes a prefix, the prefix and namespace URI pair must be added to the `XmlNamespaceManager`.  \n  \n> [!NOTE]\n>  If the XPath expression does not include a prefix, it is assumed that the namespace URI is the empty namespace. If your XML includes a default namespace, you must still add a prefix and namespace URI to the `XmlNamespaceManager`; otherwise, you will not get any nodes selected.  \n  \n For more information, see [Select Nodes Using XPath Navigation](~/docs/standard/data/xml/select-nodes-using-xpath-navigation.md). For code examples, choose an overload from the overload list in the previous section."
uid: System.Xml.XmlNode.SelectNodes*
---
