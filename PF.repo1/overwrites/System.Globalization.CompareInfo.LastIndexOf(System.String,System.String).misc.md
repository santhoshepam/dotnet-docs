---
uid: System.Globalization.CompareInfo.LastIndexOf(System.String,System.String)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters, which are characters that are not considered when performing a linguistic or culture-sensitive sort. In a culture-sensitive search, if <code>value</code> contains an ignorable character, the result is equivalent to searching with that character removed. If <code>value</code> consists only of one or more ignorable characters, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.String)"></xref> method always returns <code>source</code>.<xref href="System.String.Length"></xref> – 1, which represents the last index position in <code>source</code>. In the following example, the <xref href="System.Globalization.CompareInfo.LastIndexOf(System.String,System.String)"></xref> method is used to find three substrings (a soft hyphen (U+00AD), a soft hyphen followed by "n", and a soft hyphen followed by "m") in two strings. Only one of the strings contains a soft hyphen. In each case, because the soft hyphen is an ignorable character, the result is the same as if the soft hyphen had not been included in <code>value</code>. When searching for a soft hyphen only, the method returns 6 and 5. These values correspond to the index of the last character in the two strings.  
  
 [!code-csharp[System.Globalization.CompareInfo.LastIndexOf#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/cs/lastignorable1.cs#2)]
 [!code-vb[System.Globalization.CompareInfo.LastIndexOf#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.globalization.compareinfo.lastindexof/vb/lastignorable1.vb#2)]</p>


