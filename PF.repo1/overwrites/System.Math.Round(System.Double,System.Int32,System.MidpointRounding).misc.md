---
uid: System.Math.Round(System.Double,System.Int32,System.MidpointRounding)
additional_notes.usage: *content
---

<p>Because of the loss of precision that can result from representing decimal values as floating-point numbers or performing arithmetic operations on floating-point values, in some cases the <xref href="System.Math.Round(System.Double,System.Int32,System.MidpointRounding)"></xref> method may not appear to round midpoint values as specified by the <code>mode</code> parameter. This is illustrated in the following example, where 2.135 is rounded to 2.13 instead of 2.14. This occurs because internally the method multiplies <code>value</code> by 10<sup>digits</sup>, and the multiplication operation in this case suffers from a loss of precision.  
  
 [!code-csharp[System.Math.Round#3](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.math.round/cs/round4.cs#3)]
 [!code-vb[System.Math.Round#3](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.math.round/vb/round4.vb#3)]</p>


