---
uid: System.String.Trim(System.Char[])
additional_notes.usage: *content
---

<p>The [!INCLUDE[net_v35SP1_short](~/includes/net-v35sp1-short-md.md)] and earlier versions maintains an internal list of white-space characters that this method trims if <code>trimChars</code> is `null` or an empty array. Starting with the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)], if <code>trimChars</code> is `null` or an empty array, the method trims all Unicode white-space characters (that is, characters that produce a `true` return value when they are passed to the <xref href="System.Char.IsWhiteSpace(System.Char)"></xref> method). Because of this change, the <xref href="System.String.Trim"></xref> method in the [!INCLUDE[net_v35SP1_short](~/includes/net-v35sp1-short-md.md)] and earlier versions removes two characters, ZERO WIDTH SPACE (U+200B) and ZERO WIDTH NO-BREAK SPACE (U+FEFF), that the <xref href="System.String.Trim"></xref> method in the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)]and later versions does not remove. In addition, the <xref href="System.String.Trim"></xref> method in the [!INCLUDE[net_v35SP1_short](~/includes/net-v35sp1-short-md.md)] and earlier versions does not trim three Unicode white-space characters: MONGOLIAN VOWEL SEPARATOR (U+180E), NARROW NO-BREAK SPACE (U+202F), and MEDIUM MATHEMATICAL SPACE (U+205F).</p>


