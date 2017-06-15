---
uid: System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Globalization.CompareOptions)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> is an ignorable character, the result is equivalent to searching with that character removed. In this case, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Globalization.CompareOptions)"></xref> method always returns 0 (zero) to indicate that the match is found at the beginning of <code>source</code>. In the following example, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Globalization.CompareOptions)"></xref> method is used to search for a soft hyphen (U+00AD) in two strings. Only one of the strings contains a soft hyphen. In both cases, because the soft hyphen is an ignorable character, a culture-sensitive search returns 0 (zero) to indicate that it has found a match at the beginning of the string. An ordinal search, however, successfully finds the soft hyphen in one string and reports that it is absent from the second string.  
  
 [!code-csharp[System.Globalization.CompareInfo.IndexOf#4](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/CS/ignorable3.cs#4)]
 [!code-vb[System.Globalization.CompareInfo.IndexOf#4](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/VB/ignorable3.vb#4)]</p>


