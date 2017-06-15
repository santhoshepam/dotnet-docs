---
uid: System.String.LastIndexOf(System.String,System.Int32,System.StringComparison)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive comparison. In a culture-sensitive search (that is, if <code>comparisonType</code> is not <xref href="System.StringComparison.Ordinal"></xref> or <xref href="System.StringComparison.OrdinalIgnoreCase"></xref>), if <code>value</code> contains an ignorable character, the result is equivalent to searching with that character removed. If <code>value</code> consists only of one or more ignorable characters, the <xref href="System.String.LastIndexOf(System.String,System.Int32,System.StringComparison)"></xref> method always returns <code>startIndex</code>, which is the character position at which the search begins.  
  
 In the following example, the <xref href="System.String.LastIndexOf(System.String,System.Int32,System.StringComparison)"></xref> method is used to find the position of a soft hyphen (U+00AD) followed by an "m", starting with the final "m" in two strings. Only one of the strings contains the required substring. If the example is run on the [!INCLUDE[netfx40_short](~/includes/netfx40-short-md.md)] or later, in both cases, because the soft hyphen is an ignorable character, the method returns the index of "m" in the string when it performs a culture-sensitive comparison. Note that in the case of the first string, which includes the soft hyphen followed by an "m", the method fails to return the index of the soft hyphen but instead returns the index of the "m". The method returns the index of the soft hyphen in the first string only when it performs an ordinal comparison.  
  
 [!code-csharp[System.String.LastIndexOf#25](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.String.LastIndexOf/cs/lastindexof25.cs#25)]
 [!code-vb[System.String.LastIndexOf#25](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.String.LastIndexOf/vb/lastindexof25.vb#25)]</p>


