---
uid: System.TimeSpan.TryParse(System.String,System.TimeSpan@)
additional_notes.usage: *content
---

<p>In some cases, when a time interval component in the string to be parsed contains more than seven digits, parsing operations that succeed in the [!INCLUDE[net_v35_short](~/includes/net-v35-short-md.md)] and earlier versions may fail and throw an <xref href="System.OverflowException"></xref> in the [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)], The following example illustrates this scenario.  
  
 [!code-csharp[System.TimeSpan.TryParse#3](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.TimeSpan.TryParse/cs/tryparsefailure1.cs#3)]
 [!code-vb[System.TimeSpan.TryParse#3](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.TimeSpan.TryParse/vb/tryparsefailure1.vb#3)]</p>


