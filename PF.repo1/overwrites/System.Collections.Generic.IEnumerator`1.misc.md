---
uid: System.Collections.Generic.IEnumerator`1
additional_notes.overrides: *content
---

<p>Implementing this interface requires implementing the nongeneric <xref href="System.Collections.IEnumerator"></xref> interface. The <xref href="System.Collections.IEnumerator.MoveNext"></xref> and <xref href="System.Collections.IEnumerator.Reset"></xref> methods do not depend on <code>T</code>, and appear only on the nongeneric interface. The <xref href="System.Collections.Generic.IEnumerator`1.Current"></xref> property appears on both interfaces, and has different return types. Implement the nongeneric <xref href="System.Collections.IEnumerator.Current"></xref> property as an explicit interface implementation. This allows any consumer of the nongeneric interface to consume the generic interface.  
  
 In addition, <xref href="System.Collections.Generic.IEnumerator`1"></xref> implements <xref href="System.IDisposable"></xref>, which requires you to implement the <xref href="System.IDisposable.Dispose"></xref> method. This enables you to close database connections or release file handles or similar operations when using other resources. If there are no additional resources to dispose of, provide an empty <xref href="System.IDisposable.Dispose"></xref> implementation.</p>


