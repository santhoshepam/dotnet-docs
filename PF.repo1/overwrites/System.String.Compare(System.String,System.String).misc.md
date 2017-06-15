---
uid: System.String.Compare(System.String,System.String)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters. The <xref href="System.String.Compare(System.String,System.String)"></xref> method does not consider such characters when it performs a culture-sensitive comparison. For example, if the following code is run on the [!INCLUDE[netfx40_short](~/includes/netfx40-short-md.md)] or later, a culture-sensitive comparison of "animal" with "ani-mal" (using a soft hyphen, or U+00AD) indicates that the two strings are equivalent.  
  
 [!code-csharp[System.String.Compare#21](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.String.Compare/cs/compare21.cs#21)]
 [!code-vb[System.String.Compare#21](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.String.Compare/vb/compare21.vb#21)]  
  
 To recognize ignorable characters in a string comparison, call the <xref href="System.String.Compare(System.String,System.String,System.StringComparison)"></xref> method and supply a value of either <xref href="System.Globalization.CompareOptions.Ordinal"></xref> or <xref href="System.Globalization.CompareOptions.OrdinalIgnoreCase"></xref> for the <code>comparisonType</code> parameter.</p>


