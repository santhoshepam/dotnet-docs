---
uid: System.TimeZoneInfo.ConvertTimeToUtc(System.DateTime,System.TimeZoneInfo)
additional_notes.usage: *content
---

<p>On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, the method applies only the current adjustment rule to the time zone conversion if <code>sourceTimeZone</code> is <xref href="System.TimeZoneInfo.Local"></xref>. As a result, the method may not accurately convert times for periods before the current adjustment rule came into effect. For more information, see the Notes for Callers section in the <xref href="System.TimeZoneInfo.Local"></xref> property.</p>


