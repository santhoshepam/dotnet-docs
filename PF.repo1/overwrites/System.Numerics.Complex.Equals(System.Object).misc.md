---
uid: System.Numerics.Complex.Equals(System.Object)
additional_notes.usage: *content
---

<p>Use the <xref href="System.Numerics.Complex.Equals(System.Numerics.Complex)"></xref> method with caution, because two values that are apparently equivalent can be considered unequal due to the differing precision of their real and imaginary components. The problem can be accentuated if <code>obj</code> must be converted to a <xref href="System.Double"></xref> before performing the comparison. The following example compares a complex number whose real component appears to be equal to a <xref href="System.Single"></xref> value with that <xref href="System.Single"></xref> value. As the output shows, the comparison for equality returns `False`.  
  
 [!code-csharp[System.Numerics.Complex.Equals#8](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.numerics.complex.equals/cs/equals4.cs#8)]
 [!code-vb[System.Numerics.Complex.Equals#8](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.numerics.complex.equals/vb/equals4.vb#8)]  
  
 One recommended technique is to define an acceptable margin of difference between the two values (such as .01% of one of the values' real and imaginary components) instead of comparing the values for equality. If the absolute value of the difference between the two values is less than or equal to that margin, the difference is likely to be due to a difference in precision and, therefore, the values are likely to be equal. The following example uses this technique to compare the two values that the previous code example found to be unequal. It now finds them to be equal.  
  
 [!code-csharp[System.Numerics.Complex.Equals#7](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.numerics.complex.equals/cs/precision2.cs#7)]
 [!code-vb[System.Numerics.Complex.Equals#7](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.numerics.complex.equals/vb/precision2.vb#7)]</p>


