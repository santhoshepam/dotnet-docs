---
uid: System.TimeZoneInfo.Local
additional_notes.usage: *content
---

<p>In converting dates and times, [!INCLUDE[winxp](~/includes/winxp-md.md)] recognizes only the current adjustment rule, which it applies to all dates, including down-level dates (that is, dates that are earlier than the starting date of the current adjustment rule). On [!INCLUDE[winxp](~/includes/winxp-md.md)], to prevent local date and time information provided by the <xref href="System.TimeZoneInfo.Local"></xref> object from diverging from the date and time information displayed in the system tray, the <xref href="System.TimeZoneInfo"></xref> object returned by the <xref href="System.TimeZoneInfo.Local"></xref> property also applies the current adjustment rule to down-level dates. Applications running on [!INCLUDE[winxp](~/includes/winxp-md.md)] that require historically accurate local date and time calculations must work around this behavior by using the <xref href="System.TimeZoneInfo.FindSystemTimeZoneById(System.String)"></xref> method to retrieve a <xref href="System.TimeZoneInfo"></xref> object that corresponds to the local time zone.  
  
 The following example provides an illustration for a [!INCLUDE[winxp](~/includes/winxp-md.md)] system in the U.S. Pacific Time zone. Because the first three method calls all use the local time zone returned by the <xref href="System.TimeZoneInfo.Local"></xref> property, they apply the current time zone adjustment rule (which went into effect in 2007) to a date in 2006. The current adjustment rule provides for the transition to daylight saving time to occur on the second Sunday of March; the previous rule, which was in effect in 2006, provided for the transition to daylight saving time to occur on the first Sunday of April. Only the fourth method call, which uses the <xref href="System.TimeZoneInfo.FindSystemTimeZoneById(System.String)"></xref> method to retrieve the local time zone, accurately performs this historical date and time conversion.  
  
 [!code-csharp[System.TimeZoneInfo.ConvertTimeToUtc#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.timezoneinfo.converttimetoutc/cs/converttimetoutc.cs#1)]
 [!code-vb[System.TimeZoneInfo.ConvertTimeToUtc#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.timezoneinfo.converttimetoutc/vb/converttimetoutc.vb#1)]</p>


