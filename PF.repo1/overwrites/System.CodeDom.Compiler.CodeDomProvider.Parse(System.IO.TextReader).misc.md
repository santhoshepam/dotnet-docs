---
uid: System.CodeDom.Compiler.CodeDomProvider.Parse(System.IO.TextReader)
additional_notes.overrides: *content
---

<p>If you override this method, you must not call the corresponding method of the base class. The base-class method creates a parser in the derived class using the obsolete <xref href="System.CodeDom.Compiler.CodeDomProvider.CreateParser"></xref> method for compatibility with preexisting providers that use code parsers. The base-class method then calls the equivalent method in the <xref href="System.CodeDom.Compiler.ICodeParser"></xref> implementation to perform this function. You will get a <xref href="System.NotImplementedException"></xref> if you call the base-class method from a code provider that does not use a code parser.</p>


