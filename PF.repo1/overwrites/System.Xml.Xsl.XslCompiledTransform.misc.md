---
uid: System.Xml.Xsl.XslCompiledTransform
thread_safety: *content
---

The <xref href="System.Xml.Xsl.XslCompiledTransform"></xref> object is thread safe once it has been loaded. In other words, after the <xref href="System.Xml.Xsl.XslCompiledTransform.Load*"></xref> method has successfully completed, the <xref href="System.Xml.Xsl.XslCompiledTransform.Transform*"></xref> method can be called simultaneously from multiple threads.  
  
 If the <xref href="System.Xml.Xsl.XslCompiledTransform.Load*"></xref> method is called again in one thread while the <xref href="System.Xml.Xsl.XslCompiledTransform.Transform*"></xref> method is being called in another thread, the <xref href="System.Xml.Xsl.XslCompiledTransform"></xref> object finishes executing the <xref href="System.Xml.Xsl.XslCompiledTransform.Transform*"></xref> call by continuing to use the old state. The new state is used when the <xref href="System.Xml.Xsl.XslCompiledTransform.Load*"></xref> method successfully completes.  
  
 <block subset="none" type="note"><p>  
 The <xref href="System.Xml.Xsl.XslCompiledTransform.Load*"></xref> method is not thread safe when called simultaneously from multiple threads.  
  
</p></block>


