---
summary: Validates that an <xref href="System.Xml.Linq.XDocument"></xref>, an <xref href="System.Xml.Linq.XElement"></xref>, or an <xref href="System.Xml.Linq.XAttribute"></xref> conforms to an XSD in an <xref href="System.Xml.Schema.XmlSchemaSet"></xref>.
remarks: "These methods use an underlying <xref:System.Xml.XmlReader> to validate the XML tree against an XSD.  \n  \n Validation error and warning messages are handled using the <xref:System.Xml.Schema.ValidationEventHandler> delegate. If no event handler is provided to these methods, validation errors are exposed as an <xref:System.Xml.Schema.XmlSchemaValidationException>. Validation warnings do not cause an <xref:System.Xml.Schema.XmlSchemaValidationException> to be thrown.  \n  \n Some of these extension methods optionally allow population of the post-schema-validation infoset (PSVI)."
uid: System.Xml.Schema.Extensions.Validate*
---
