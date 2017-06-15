---
uid: System.Globalization.CompareInfo.LastIndexOf(System.String,System.Char,System.Globalization.CompareOptions)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> is an ignorable character, the result is equivalent to searching with that character removed. In this case, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.Char,System.Globalization.CompareOptions)"></xref> method always returns the last character position in <code>source</code> to indicate that the match is found at the end of <code>source</code>. In the following example, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.Char,System.Globalization.CompareOptions)"></xref> method is used to search for a soft hyphen (U+00AD) in two strings. Only one of the strings contains a soft hyphen. In both cases, because the soft hyphen is an ignorable character, a culture-sensitive search returns the last index position in the source string. In contrast, an ordinal search successfully finds the soft hyphen in one string and reports that it is absent from the second string.  
  
 [!code-csharp[System.Globalization.CompareInfo.LastIndexOf#4](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/cs/lastignorable3.cs#4)]
 [!code-vb[System.Globalization.CompareInfo.LastIndexOf#4](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/vb/lastignorable3.vb#4)]</p>


