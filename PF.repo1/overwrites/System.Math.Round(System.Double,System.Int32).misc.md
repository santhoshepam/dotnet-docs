---
uid: System.Math.Round(System.Double,System.Int32)
additional_notes.usage: *content
---

<p>Because of the loss of precision that can result from representing decimal values as floating-point numbers or performing arithmetic operations on floating-point values, in some cases the <xref href="System.Math.Round(System.Double,System.Int32)"></xref> method may not appear to round midpoint values to the nearest even value in the <code>digits</code> decimal position. This is illustrated in the following example, where 2.135 is rounded to 2.13 instead of 2.14. This occurs because internally the method multiplies <code>value</code> by 10<sup>digits</sup>, and the multiplication operation in this case suffers from a loss of precision.  
  
 [!code-csharp[System.Math.Round#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.math.round/cs/round3.cs#2)]
 [!code-vb[System.Math.Round#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.math.round/vb/round3.vb#2)]</p>


