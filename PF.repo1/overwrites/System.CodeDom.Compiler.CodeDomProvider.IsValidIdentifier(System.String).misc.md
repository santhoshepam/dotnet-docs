---
uid: System.CodeDom.Compiler.CodeDomProvider.IsValidIdentifier(System.String)
additional_notes.overrides: *content
---

<p>When overriding <xref href="System.CodeDom.Compiler.CodeDomProvider.IsValidIdentifier(System.String)"></xref> in a derived class, design the method to return `true` only if the value fits the rules of the language and does not conflict with a keyword.  
  
 If you override this method, you must not call the corresponding method of the base class. The base-class method creates a generator in the derived class using the obsolete <xref href="System.CodeDom.Compiler.CodeDomProvider.CreateGenerator"></xref> method for compatibility with preexisting providers that use code generators. The base-class method then calls the equivalent method in the <xref href="System.CodeDom.Compiler.ICodeGenerator"></xref> implementation to perform this function. You will get a <xref href="System.NotImplementedException"></xref> if you call the base-class method from a code provider that does not use a code generator.</p>


