---
uid: System.Double.Equals(System.Object)
additional_notes.usage: *content
---

<p>Compiler overload resolution may account for an apparent difference in the behavior of the two <xref href="System.Double.Equals(System.Object)"></xref> method overloads. If an implicit conversion between the <code>obj</code> argument and a <xref href="System.Double"></xref> is defined and the argument is not typed as an <xref href="System.Object"></xref>, compilers may perform an implicit conversion and call the <xref href="System.Double.Equals(System.Double)"></xref> method. Otherwise, they call the <xref href="System.Double.Equals(System.Object)"></xref> method, which always returns `false` if its <code>obj</code> argument is not a <xref href="System.Double"></xref> value. The following example illustrates the difference in behavior between the two method overloads. In the case of all primitive numeric types except for <xref href="System.Decimal"></xref> and in C#, the first comparison returns `true` because the compiler automatically performs a widening conversion and calls the <xref href="System.Double.Equals(System.Double)"></xref> method, whereas the second comparison returns `false` because the compiler calls the <xref href="System.Double.Equals(System.Object)"></xref> method.  
  
 [!code-csharp[System.Double.Equals#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.double.equals/cs/equalsoverl.cs#2)]
 [!code-vb[System.Double.Equals#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.double.equals/vb/equalsoverl.vb#2)]</p>


