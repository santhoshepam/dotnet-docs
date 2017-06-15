---
summary: Executes the XSLT transformation.
remarks: >-
  > [!NOTE]

  >  There are differences between XSLT compiled in Debug mode and XSLT compiled in Release mode. In some situations, style sheets compiled in Debug mode will not throw errors during <xref:System.Xml.Xsl.XslCompiledTransform.Load%2A>, but will later fail during <xref:System.Xml.Xsl.XslCompiledTransform.Transform%2A>. The same style sheet compiled in Release mode will fail during <xref:System.Xml.Xsl.XslCompiledTransform.Load%2A>. An example of such behavior is when a variable that is not of a node-set type is assigned to an expression where a node-set is required.
uid: System.Xml.Xsl.XslCompiledTransform.Transform*
---
