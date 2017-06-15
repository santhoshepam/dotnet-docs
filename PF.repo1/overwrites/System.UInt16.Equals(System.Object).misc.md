---
uid: System.UInt16.Equals(System.Object)
additional_notes.usage: *content
---

<p>Compiler overload resolution may account for an apparent difference in the behavior of the two <xref href="System.UInt16.Equals(System.UInt16)"></xref> method overloads. If an implicit conversion between the <code>obj</code> argument and a <xref href="System.UInt16"></xref> is defined and the argument is not typed as an <xref href="System.Object"></xref>, compilers perform an implicit conversion and call the <xref href="System.UInt16.Equals(System.UInt16)"></xref> method. Otherwise, they call the <xref href="System.UInt16.Equals(System.Object)"></xref> method, which always returns `false` if its <code>obj</code> argument is not a <xref href="System.UInt16"></xref> value. The following example illustrates the difference in behavior between the two method overloads. In the case of a <xref href="System.Byte"></xref> value, the first comparison returns `true` because the compiler automatically performs a widening conversion and calls the <xref href="System.UInt16.Equals(System.UInt16)"></xref> method, whereas the second comparison returns `false` because the compiler calls the <xref href="System.UInt16.Equals(System.Object)"></xref> method.  
  
 [!code-csharp[System.UInt16.Equals#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.uint16.equals/cs/equalsoverl.cs#1)]
 [!code-vb[System.UInt16.Equals#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.uint16.equals/vb/equalsoverl.vb#1)]</p>


