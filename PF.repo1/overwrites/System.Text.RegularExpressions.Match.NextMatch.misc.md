---
uid: System.Text.RegularExpressions.Match.NextMatch
additional_notes.usage: *content
---

<p>When a match attempt is repeated by calling the <xref href="System.Text.RegularExpressions.Match.NextMatch"></xref> method, the regular expression engine gives empty matches special treatment. Usually, <xref href="System.Text.RegularExpressions.Match.NextMatch"></xref> begins the search for the next match exactly where the previous match left off. However, after an empty match, the <xref href="System.Text.RegularExpressions.Match.NextMatch"></xref> method advances by one character before trying the next match. This behavior guarantees that the regular expression engine will progress through the string. Otherwise, because an empty match does not result in any forward movement, the next match would start in exactly the same place as the previous match, and it would match the same empty string repeatedly.  
  
 The following example provides an illustration. The regular expression pattern <code>a*</code> searches for zero or more occurrences of the letter "a" in the string "abaabb". As the output from the example shows, the search finds six matches. The first match attempt finds the first "a". The second match starts exactly where the first match ends, before the first b; it finds zero occurrences of "a" and returns an empty string. The third match does not begin exactly where the second match ended, because the second match returned an empty string. Instead, it begins one character later, after the first "b". The third match finds two occurrences of "a" and returns "aa". The fourth match attempt begins where the third match ended, before the second "b", and returns an empty string. The fifth match attempt again advances one character so that it begins before the third "b" and returns an empty string. The sixth match begins after the last "b" and returns an empty string again.  
  
 [!code-csharp[System.Text.RegularExpressions.Match.NextMatch#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.text.regularexpressions.match.nextmatch/cs/nextmatch1.cs#1)]
 [!code-vb[System.Text.RegularExpressions.Match.NextMatch#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.text.regularexpressions.match.nextmatch/vb/nextmatch1.vb#1)]</p>


