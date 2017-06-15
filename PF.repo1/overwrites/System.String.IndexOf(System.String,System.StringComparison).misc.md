---
uid: System.String.IndexOf(System.String,System.StringComparison)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive comparison. In a culture-sensitive search (that is, if <code>comparisonType</code> is not <xref href="System.StringComparison.Ordinal"></xref> or <xref href="System.StringComparison.OrdinalIgnoreCase"></xref>), if <code>value</code> contains an ignorable character, the result is equivalent to searching with that character removed. If <code>value</code> consists only of one or more ignorable characters, the <xref href="System.String.IndexOf(System.String,System.StringComparison)"></xref> method always returns 0 (zero) to indicate that the match is found at the beginning of the current instance.  
  
 In the following example, the <xref href="System.String.IndexOf(System.String,System.StringComparison)"></xref> method is used to find three substrings (a soft hyphen (U+00AD), a soft hyphen followed by "n", and a soft hyphen followed by "m") in two strings. Only one of the strings contains a soft hyphen. If the example is run on the [!INCLUDE[netfx40_short](~/includes/netfx40-short-md.md)] or later, because the soft hyphen is an ignorable character, a culture-sensitive search returns the same value that it would return if the soft hyphen were not included in the search string. An ordinal search, however, successfully finds the soft hyphen in one string and reports that it is absent from the second string.  
  
 [!code-csharp[System.String.IndexOf#26](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.String.IndexOf/CS/ignorable26.cs#26)]
 [!code-vb[System.String.IndexOf#26](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.String.IndexOf/VB/ignorable26.vb#26)]</p>


