---
uid: System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Int32,System.Int32)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> is an ignorable character, the result is equivalent to searching with that character removed. In this case, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Int32,System.Int32)"></xref> method always returns <code>startIndex</code>, which is the character position at which the search first began. In the following example, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.Char,System.Int32,System.Int32)"></xref> method is used to find a soft hyphen (U+00AD) after an "n" in two strings. Only one of the strings contains a soft hyphen. In both cases, because the soft hyphen is an ignorable character, the method returns 1 to indicate that it has found a match at the position of the "n".  
  
 [!code-csharp[System.Globalization.CompareInfo.IndexOf#9](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/CS/ignorable8.cs#9)]
 [!code-vb[System.Globalization.CompareInfo.IndexOf#9](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/VB/ignorable8.vb#9)]</p>


