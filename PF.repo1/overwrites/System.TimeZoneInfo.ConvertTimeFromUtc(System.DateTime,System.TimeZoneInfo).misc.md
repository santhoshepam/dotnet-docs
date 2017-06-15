---
uid: System.TimeZoneInfo.ConvertTimeFromUtc(System.DateTime,System.TimeZoneInfo)
additional_notes.usage: *content
---

<p>On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, this method applies only the current adjustment rule to the time zone conversion if <code>destinationTimeZone</code> is <xref href="System.TimeZoneInfo.Local"></xref>. As a result, the method may not accurately convert times for periods before the current adjustment rule came into effect. For more information, see the Notes for Callers section in the <xref href="System.TimeZoneInfo.Local"></xref> property.</p>


