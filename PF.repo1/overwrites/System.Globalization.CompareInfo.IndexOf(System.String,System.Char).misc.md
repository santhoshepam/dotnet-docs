---
uid: System.Globalization.CompareInfo.IndexOf(System.String,System.Char)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> is an ignorable character, the result is equivalent to searching with that character removed. In this case, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char)"></xref> method always returns 0 (zero) to indicate that the match is found at the beginning of <code>source</code>. In the following example, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char)"></xref> method is used to find the soft hyphen (U+00AD) in two strings. Only one of the strings contains a soft hyphen. In both cases, because the soft hyphen is an ignorable character, the method returns 0 (zero) to indicate that it has found a match at the beginning of the string.  
  
 [!code-csharp[System.Globalization.CompareInfo.IndexOf#3](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/CS/ignorable2.cs#3)]
 [!code-vb[System.Globalization.CompareInfo.IndexOf#3](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/VB/ignorable2.vb#3)]</p>


