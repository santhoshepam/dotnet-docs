---
uid: System.IEquatable`1.Equals(`0)
additional_notes.overrides: *content
---

<p>If you implement <xref href="System.IEquatable`1.Equals(`0)"></xref>, you should also override the base class implementations of <xref href="System.Object.Equals(System.Object)"></xref> and <xref href="System.Object.GetHashCode"></xref> so that their behavior is consistent with that of the <xref href="System.IEquatable`1.Equals(`0)"></xref> method. If you do override <xref href="System.Object.Equals(System.Object)"></xref>, your overridden implementation is also called in calls to the static `Equals(System.Object, System.Object)` method on your class. In addition, you should overload the `op_Equality` and `op_Inequality` operators. This ensures that all tests for equality return consistent results, which the example illustrates.</p>


