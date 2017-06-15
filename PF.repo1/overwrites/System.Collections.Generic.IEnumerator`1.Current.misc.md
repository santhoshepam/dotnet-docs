---
uid: System.Collections.Generic.IEnumerator`1.Current
additional_notes.overrides: *content
---

<p>Implementing this interface requires implementing the nongeneric <xref href="System.Collections.IEnumerator"></xref> interface. The <xref href="System.Collections.Generic.IEnumerator`1.Current"></xref> property appears on both interfaces, and has different return types. Implement the nongeneric <xref href="System.Collections.IEnumerator.Current"></xref> property as an explicit interface implementation. This allows any consumer of the nongeneric interface to consume the generic interface.</p>


