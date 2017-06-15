---
uid: System.Single.Equals(System.Object)
additional_notes.usage: *content
---

<p>Compiler overload resolution may account for an apparent difference in the behavior of the two <xref href="System.Single.Equals(System.Object)"></xref> method overloads. If an implicit conversion between the <code>obj</code> argument and a <xref href="System.Single"></xref> is defined and the argument is not typed as an <xref href="System.Object"></xref>, compilers may perform an implicit conversion and call the <xref href="System.Single.Equals(System.Single)"></xref> method. Otherwise, they call the <xref href="System.Single.Equals(System.Object)"></xref> method, which always returns `false` if its <code>obj</code> argument is not a <xref href="System.Single"></xref> value. The following example illustrates the difference in behavior between the two method overloads. In the case of all primitive numeric types except for <xref href="System.Double"></xref> in Visual Basic and except for <xref href="System.Decimal"></xref> and <xref href="System.Double"></xref> in C#, the first comparison returns `true` because the compiler automatically performs a widening conversion and calls the <xref href="System.Single.Equals(System.Single)"></xref> method, whereas the second comparison returns `false` because the compiler calls the <xref href="System.Single.Equals(System.Object)"></xref> method.  
  
 [!code-csharp[System.Single.Equals#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.single.equals/cs/equalsoverl.cs#2)]
 [!code-vb[System.Single.Equals#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.single.equals/vb/equalsoverl.vb#2)]</p>


