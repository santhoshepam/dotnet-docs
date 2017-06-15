---
uid: System.String.CompareTo(System.Object)
additional_notes.usage: *content
---

<p>Character sets include ignorable characters. The <xref href="System.String.CompareTo(System.Object)"></xref> method does not consider such characters when it performs a culture-sensitive comparison. For example, if the following code is run on the [!INCLUDE[netfx40_short](~/includes/netfx40-short-md.md)] or later, a comparison of "animal" with "ani-mal" (using a soft hyphen, or U+00AD) indicates that the two strings are equivalent.  
  
 [!code-csharp[System.String.CompareTo#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.string.compareto/cs/compareto1.cs#1)]
 [!code-vb[System.String.CompareTo#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.string.compareto/vb/compareto1.vb#1)]  
  
 To recognize ignorable characters in a string comparison, call the <xref href="System.String.CompareOrdinal(System.String,System.String)"></xref> method.</p>


