---
uid: System.DateTime.ToUniversalTime
additional_notes.usage: *content
---

<p>The <xref href="System.DateTime.ToUniversalTime"></xref> method is sometimes used to convert a local time to UTC. The <xref href="System.DateTime.ToLocalTime"></xref> method is then called to restore the original local time. However, if the original time represents an invalid time in the local time zone, the two local time values will not be equal. For additional information and an example, see the <xref href="System.DateTime.ToLocalTime"></xref> method.  
  
 On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, the <xref href="System.DateTime.ToUniversalTime"></xref> method recognizes only the current adjustment rule for the local time zone, which it applies to all dates, including down-level dates (that is, dates that are earlier than the starting date of the current adjustment rule). Applications running on [!INCLUDE[winxp](~/includes/winxp-md.md)] that require historically accurate local date and time calculations must work around this behavior by using the <xref href="System.TimeZoneInfo.FindSystemTimeZoneById(System.String)"></xref> method to retrieve a <xref href="System.TimeZoneInfo"></xref> object that corresponds to the local time zone and calling its <xref href="System.TimeZoneInfo.ConvertTimeToUtc(System.DateTime,System.TimeZoneInfo)"></xref> method.  
  
 The following example illustrates the difference between the <xref href="System.DateTime.ToUniversalTime"></xref> and <xref href="System.TimeZoneInfo.ConvertTimeToUtc(System.DateTime,System.TimeZoneInfo)"></xref> methods on a [!INCLUDE[winxp](~/includes/winxp-md.md)] system in the U.S. Pacific Time zone. The first two method calls apply the current time zone adjustment rule (which went into effect in 2007) to a date in 2006. The current adjustment rule provides for the transition to daylight saving time on the second Sunday of March; the previous rule, which was in effect in 2006, provided for the transition to daylight saving time to occur on the first Sunday of April. Only the third method call accurately performs this historical date and time conversion.  
  
 [!code-csharp[System.DateTime.ToUniversalTime#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.datetime.touniversaltime/cs/touniversaltime.cs#1)]
 [!code-vb[System.DateTime.ToUniversalTime#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.datetime.touniversaltime/vb/touniversaltime.vb#1)]</p>


