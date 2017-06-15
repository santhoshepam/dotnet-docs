---
uid: System.Double.ToString(System.String)
additional_notes.usage: *content
---

<p>In some cases, <xref href="System.Double"></xref> values formatted with the "R" standard numeric format string do not successfully round-trip if compiled using the `/platform:x64` or `/platform:anycpu` switches and run on 64-bit systems. To work around this problem, you can format <xref href="System.Double"></xref> values by using the "G17" standard numeric format string. The following example uses the "R" format string with a <xref href="System.Double"></xref> value that does not round-trip successfully, and also uses the "G17" format string to successfully round-trip the original value.  
  
 [!code-csharp[System.Double.ToString#6](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Double.ToString/cs/roundtripex2.cs#6)]
 [!code-vb[System.Double.ToString#6](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Double.ToString/vb/roundtripex2.vb#6)]</p>


