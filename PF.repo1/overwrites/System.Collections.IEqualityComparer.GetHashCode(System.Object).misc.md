---
uid: System.Collections.IEqualityComparer.GetHashCode(System.Object)
additional_notes.overrides: *content
---

<p>Implementations are required to ensure that if the <xref href="System.Collections.IEqualityComparer.Equals(System.Object,System.Object)"></xref> method returns `true` for two objects <code>x</code> and <code>y</code>, then the value returned by the <xref href="System.Collections.IEqualityComparer.GetHashCode(System.Object)"></xref> method for <code>x</code> must equal the value returned for <code>y</code>.</p>


