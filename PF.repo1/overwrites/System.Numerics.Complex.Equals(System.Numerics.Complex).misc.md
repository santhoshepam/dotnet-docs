---
uid: System.Numerics.Complex.Equals(System.Numerics.Complex)
additional_notes.usage: *content
---

<p>Use the <xref href="System.Numerics.Complex.Equals(System.Numerics.Complex)"></xref> method with caution, because two values that are apparently equivalent can be considered unequal due to the differing precision of their real and imaginary components. The following example reports that <code>(3.33333, 0.142857)</code> and <code>(10/3, 1/7)</code> are not equal.  
  
 [!code-csharp[System.Numerics.Complex.Equals#4](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.numerics.complex.equals/cs/precision1.cs#4)]
 [!code-vb[System.Numerics.Complex.Equals#4](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.numerics.complex.equals/vb/precision1.vb#4)]  
  
 One recommended technique is to define an acceptable margin of difference between the two values (such as .01% of one of the values' real and imaginary components) instead of comparing the values for equality. If the absolute value of the difference between the two values is less than or equal to that margin, the difference is likely to be due to a difference in precision, and, therefore, the values are likely to be equal. The following example uses this technique to compare the two complex values that the previous code example found to be unequal. It finds the two complex numbers to be equal.  
  
 [!code-csharp[System.Numerics.Complex.Equals#5](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.numerics.complex.equals/cs/precision1.cs#5)]
 [!code-vb[System.Numerics.Complex.Equals#5](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.numerics.complex.equals/vb/precision1.vb#5)]</p>


