---
uid: System.Globalization.CompareInfo.IndexOf(System.String,System.String,System.Int32,System.Int32)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> contains an ignorable character, the result is equivalent to searching with that character removed. If <code>value</code> consists only of one or more ignorable characters, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.String,System.Int32,System.Int32)"></xref> method always returns <code>startIndex</code>, which is the character position at which the search begins.  
  
 In the following example, the <xref href="System.Globalization.CompareInfo.IndexOf(System.String,System.String,System.Int32,System.Int32)"></xref> method is used to find the position of a soft hyphen (U+00AD) followed by an "m" starting in the third through sixth character positions in two strings. Only one of the strings contains the required substring. In both cases, because the soft hyphen is an ignorable character, the method returns the index of "m" in the string when it performs a culture-sensitive comparison. Note that in the case of the first string, which includes the soft hyphen followed by an "m", the method fails to return the index of the soft hyphen but instead returns the index of the "m".  
  
 [!code-csharp[System.Globalization.CompareInfo.IndexOf#17](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/CS/ignorable16.cs#17)]
 [!code-vb[System.Globalization.CompareInfo.IndexOf#17](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Globalization.CompareInfo.IndexOf/VB/ignorable16.vb#17)]</p>


