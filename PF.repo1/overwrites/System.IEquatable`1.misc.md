---
uid: System.IEquatable`1
additional_notes.overrides: *content
---

<p>Replace the type parameter of the <xref href="System.IEquatable`1"></xref> interface with the type that is implementing this interface.  
  
 If you implement <xref href="System.IEquatable`1"></xref>, you should also override the base class implementations of <xref href="System.Object.Equals(System.Object)"></xref> and <xref href="System.Object.GetHashCode"></xref> so that their behavior is consistent with that of the <xref href="System.IEquatable`1.Equals(`0)"></xref> method. If you do override <xref href="System.Object.Equals(System.Object)"></xref>, your overridden implementation is also called in calls to the static `Equals(System.Object, System.Object)` method on your class. In addition, you should overload the `op_Equality` and `op_Inequality` operators. This ensures that all tests for equality return consistent results.  
  
 <block subset="none" type="note"><p>  
 For information on overriding <xref href="System.Object.Equals(System.Object)"></xref>, see the <xref href="System.Object.Equals(System.Object)"></xref> article.  
  
</p></block>  
  
 For a value type, you should always implement <xref href="System.IEquatable`1"></xref> and override <xref href="System.Object.Equals(System.Object)"></xref> for better performance. <xref href="System.Object.Equals(System.Object)"></xref> boxes value types and relies on reflection to compare two values for equality. Both your implementation of <xref href="System.IEquatable`1.Equals(`0)"></xref> and your override of <xref href="System.Object.Equals(System.Object)"></xref> should return consistent results.  
  
 If you implement <xref href="System.IEquatable`1"></xref>, you should also implement <xref href="System.IComparable`1"></xref> if instances of your type can be ordered or sorted. If your type implements <xref href="System.IComparable`1"></xref>, you should also always implement <xref href="System.IEquatable`1"></xref>.</p>


