---
uid: System.Globalization.CompareInfo.Compare(System.String,System.String)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive comparison. The <xref href="System.Globalization.CompareInfo.Compare(System.String,System.String)"></xref> method does not consider such characters when it performs a culture-sensitive comparison. For instance, a culture-sensitive comparison of "animal" with "ani-mal" (using a soft hyphen, or U+00AD) indicates that the two strings are equivalent, as the following example shows.  
  
 [!code-vb[System.Globalization.CompareInfo.Compare#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.globalization.compareinfo.compare/vb/compare1.vb#1)]  
  
 To recognize ignorable characters in a string comparison, call the <xref href="System.Globalization.CompareInfo.Compare(System.String,System.String,System.Globalization.CompareOptions)"></xref> method and supply a value of either <xref href="System.Globalization.CompareOptions.Ordinal"></xref> or <xref href="System.Globalization.CompareOptions.OrdinalIgnoreCase"></xref> for the <code>options</code> parameter.</p>


