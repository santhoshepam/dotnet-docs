---
uid: System.String.Compare(System.String,System.String,System.Boolean,System.Globalization.CultureInfo)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters. The <xref href="System.String.Compare(System.String,System.String,System.Boolean,System.Globalization.CultureInfo)"></xref> method does not consider such characters when it performs a culture-sensitive comparison. For example, if the following code is run on the [!INCLUDE[netfx40_short](~/includes/netfx40-short-md.md)] or later, a case-insensitive comparison of "animal" with "Ani-mal" (using a soft hyphen, or U+00AD) using the invariant culture indicates that the two strings are equivalent.  
  
 [!code-csharp[System.String.Compare#23](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.String.Compare/cs/compare23.cs#23)]
 [!code-vb[System.String.Compare#23](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.String.Compare/vb/compare23.vb#23)]  
  
 To recognize ignorable characters in a string comparison, call the <xref href="System.String.Compare(System.String,System.String,System.Globalization.CultureInfo,System.Globalization.CompareOptions)"></xref> method and supply a value of either <xref href="System.Globalization.CompareOptions.Ordinal"></xref> or <xref href="System.Globalization.CompareOptions.OrdinalIgnoreCase"></xref> for the <code>options</code> parameter.</p>


