---
uid: System.String.Split(System.String[],System.StringSplitOptions)
additional_notes.usage: *content
---

<p>In the [!INCLUDE[net_v35_short](~/includes/net-v35-short-md.md)] and earlier versions, if the <xref href="System.String.Split(System.Char[])"></xref> method is passed a <code>separator</code> that is `null` or contains no characters, the method uses a slightly different set of characters to split the string than the <xref href="System.String.Trim(System.Char[])"></xref> method does to trim the string. In the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)], both methods use an identical set of Unicode white-space characters.</p>


