---
uid: System.Int32.Equals(System.Int32)
additional_notes.usage: *content
---

<p>Compiler overload resolution may account for an apparent difference in the behavior of the two <xref href="System.Int32.Equals(System.Int32)"></xref> method overloads. If an implicit conversion between the <code>obj</code> argument and an <xref href="System.Int32"></xref> is defined and the argument is not typed as an <xref href="System.Object"></xref>, compilers perform an implicit conversion and call the <xref href="System.Int32.Equals(System.Int32)"></xref> method. Otherwise, they call the <xref href="System.Int32.Equals(System.Object)"></xref> method, which always returns `false` if its <code>obj</code> argument is not an <xref href="System.Int32"></xref> value. The following example illustrates the difference in behavior between the two method overloads. In the case of the <xref href="System.Byte"></xref>, <xref href="System.Int16"></xref>, <xref href="System.SByte"></xref>, and <xref href="System.UInt16"></xref> values, the first comparison returns `true` because the compiler automatically performs a widening conversion and calls the <xref href="System.Int32.Equals(System.Int32)"></xref> method, whereas the second comparison returns `false` because the compiler calls the <xref href="System.Int32.Equals(System.Object)"></xref> method.  
  
 [!code-csharp[System.Int32.Equals#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.int32.equals/cs/equalsoverloads2.cs#1)]
 [!code-vb[System.Int32.Equals#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.int32.equals/vb/equalsoverloads2.vb#1)]</p>


