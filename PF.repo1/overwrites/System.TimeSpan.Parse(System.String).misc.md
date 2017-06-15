---
uid: System.TimeSpan.Parse(System.String)
additional_notes.usage: *content
---

<p>When a time interval component in the string to be parsed contains more than seven digits, parsing operations in the [!INCLUDE[net_v35_short](~/includes/net-v35-short-md.md)] and earlier versions may behave differently from parsing operations in the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)]. In some cases, parsing operations that succeed in the [!INCLUDE[net_v35_short](~/includes/net-v35-short-md.md)] and earlier versions may fail and throw an <xref href="System.OverflowException"></xref> in the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)]. In other cases, parsing operations that throw a <xref href="System.FormatException"></xref> in the [!INCLUDE[net_v35_short](~/includes/net-v35-short-md.md)] and earlier versions may fail and throw an <xref href="System.OverflowException"></xref> in the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)]. The following example illustrates both scenarios.  
  
 [!code-csharp[System.TimeSpan.Parse#3](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.timespan.parse/cs/parsefailure1.cs#3)]
 [!code-vb[System.TimeSpan.Parse#3](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.timespan.parse/vb/parsefailure1.vb#3)]</p>


