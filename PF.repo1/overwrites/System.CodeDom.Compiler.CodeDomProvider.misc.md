---
uid: System.CodeDom.Compiler.CodeDomProvider
additional_notes.overrides: *content
---

<p>In the .NET Framework versions 1.0 and 1.1, code providers consist of implementations of <xref href="System.CodeDom.Compiler.CodeDomProvider"></xref>, <xref href="System.CodeDom.Compiler.ICodeGenerator"></xref>, <xref href="System.CodeDom.Compiler.ICodeParser"></xref>, and <xref href="System.CodeDom.Compiler.ICodeCompiler"></xref>. In the [!INCLUDE[dnprdnlong](~/includes/dnprdnlong-md.md)], the <xref href="System.CodeDom.Compiler.CodeDomProvider.CreateGenerator"></xref>, <xref href="System.CodeDom.Compiler.CodeDomProvider.CreateParser"></xref>, and <xref href="System.CodeDom.Compiler.CodeDomProvider.CreateCompiler"></xref> methods are obsolete, and the methods of <xref href="System.CodeDom.Compiler.ICodeGenerator"></xref> and <xref href="System.CodeDom.Compiler.ICodeCompiler"></xref> are directly available in the <xref href="System.CodeDom.Compiler.CodeDomProvider"></xref> class. You should override those methods in your code provider implementation and not call the base methods.</p>


