---
uid: System.Globalization.CompareInfo.LastIndexOf(System.String,System.Char,System.Int32,System.Int32,System.Globalization.CompareOptions)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> is an ignorable character, the result is equivalent to searching with that character removed. In this case, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.Char,System.Int32,System.Int32,System.Globalization.CompareOptions)"></xref> method always returns <code>startIndex</code>, which is the character position at which the search begins. In the following example, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.Char,System.Int32,System.Int32,System.Globalization.CompareOptions)"></xref> method is used to find a soft hyphen (U+00AD) that precedes the final "m" in two strings. Only one of the strings contains a soft hyphen. In both cases, because the soft hyphen is an ignorable character, a culture-sensitive search returns the index position of the "m", which is the value of <code>startIndex</code>. An ordinal search, however, successfully finds the soft hyphen in one string and reports that it is absent from the second string.  
  
 [!code-csharp[System.Globalization.CompareInfo.LastIndexOf#12](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/cs/lastignorable11.cs#12)]
 [!code-vb[System.Globalization.CompareInfo.LastIndexOf#12](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/vb/lastignorable11.vb#12)]</p>


