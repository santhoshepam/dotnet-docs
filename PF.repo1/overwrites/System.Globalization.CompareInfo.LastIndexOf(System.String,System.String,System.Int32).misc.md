---
uid: System.Globalization.CompareInfo.LastIndexOf(System.String,System.String,System.Int32)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> contains an ignorable character, the result is equivalent to searching with that character removed. If <code>value</code> consists only of one or more ignorable characters, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.String,System.Int32)"></xref> method always returns <code>startIndex</code>, which is the character position at which the search begins. In the following example, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.String,System.Int32)"></xref> method is used to find a substring that includes a soft hyphen (U+00AD) and that precedes or includes the final "m" in a string. Because the soft hyphen in the search string is ignored, calling the method to find a substring that consists of the soft hyphen and "m" returns the position of the "m" in the string, whereas calling it to find a substring that consists of the soft hyphen and "n" returns the position of the "n". When the search string contains only the soft hyphen, the method returns the index of the "m", which represents the value of <code>startIndex</code>.  
  
 [!code-csharp[System.Globalization.CompareInfo.LastIndexOf#7](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/cs/lastignorable6.cs#7)]
 [!code-vb[System.Globalization.CompareInfo.LastIndexOf#7](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/vb/lastignorable6.vb#7)]</p>


