---
summary: Loads the `XmlDataDocument` using the specified data source and synchronizes the <xref href="System.Data.DataSet"></xref> with the loaded data.
remarks: "> [!NOTE]\n>  In order to view the XML data relationally, you must first specify a schema to use for data mapping. This can be done either by calling the <xref:System.Data.DataSet.ReadXmlSchema%2A> method or by creating the tables and columns within the `DataSet` manually. This step must be done before calling `Load`.  \n  \n `XmlDataDocument` does not support creating entity references. If the data includes entity references, the `Load` method resolves and expands any entity references. However, if you are using the `Load` overload that takes a <xref:System.Xml.XmlReader> as an argument, you must specify an `XmlReader` that can resolve entities."
uid: System.Xml.XmlDataDocument.Load*
---
