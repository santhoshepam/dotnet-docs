---
uid: System.Collections.Generic.IEqualityComparer`1.Equals(`0,`0)
additional_notes.overrides: *content
---

<p>Implementations are required to ensure that if the <xref href="System.Collections.Generic.IEqualityComparer`1.Equals(`0,`0)"></xref> method returns `true` for two objects <code>x</code> and <code>y</code>, then the value returned by the <xref href="System.Collections.Generic.IEqualityComparer`1.GetHashCode(`0)"></xref> method for <code>x</code> must equal the value returned for <code>y</code>.  
  
 The <xref href="System.Collections.Generic.IEqualityComparer`1.Equals(`0,`0)"></xref> method is reflexive, symmetric, and transitive. That is, it returns `true` if used to compare an object with itself; `true` for two objects <code>x</code> and <code>y</code> if it is `true` for <code>y</code> and <code>x</code>; and `true` for two objects <code>x</code> and <code>z</code> if it is `true` for <code>x</code> and <code>y</code> and also `true` for <code>y</code> and <code>z</code>.</p>


