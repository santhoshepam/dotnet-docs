---
uid: System.CodeDom.Compiler.CodeDomProvider.GenerateCodeFromStatement(System.CodeDom.CodeStatement,System.IO.TextWriter,System.CodeDom.Compiler.CodeGeneratorOptions)
additional_notes.overrides: *content
---

<p>If you override this method, you must not call the corresponding method of the base class. The base-class method creates a generator in the derived class using the obsolete <xref href="System.CodeDom.Compiler.CodeDomProvider.CreateGenerator"></xref> method for compatibility with preexisting providers that use code generators. The base-class method then calls the equivalent method in the <xref href="System.CodeDom.Compiler.ICodeGenerator"></xref> implementation to perform this function. You will get a <xref href="System.NotImplementedException"></xref> if you call the base-class method from a code provider that does not use a code generator.</p>


