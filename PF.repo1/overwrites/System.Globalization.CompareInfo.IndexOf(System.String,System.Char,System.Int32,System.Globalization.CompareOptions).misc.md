---
uid: System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Int32,System.Globalization.CompareOptions)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> is an ignorable character, the result is equivalent to searching with that character removed. In this case, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Int32,System.Globalization.CompareOptions)"></xref> method always returns <code>startIndex</code>, the character position at which the search first began. In the following example, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Int32,System.Globalization.CompareOptions)"></xref> method is used to find the soft hyphen (U+00AD) after an "n" in two strings. Only one of the strings contains a soft hyphen. In both cases, because the soft hyphen is an ignorable character, a culture-sensitive search returns 1 to indicate that it has found a match at the position of the "n". An ordinal search, however, successfully finds the soft hyphen in one string and reports that it is absent from the second string.  
  
 [!code-csharp[System.Globalization.CompareInfo.IndexOf#8](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/CS/ignorable7.cs#8)]
 [!code-vb[System.Globalization.CompareInfo.IndexOf#8](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/VB/ignorable7.vb#8)]</p>


