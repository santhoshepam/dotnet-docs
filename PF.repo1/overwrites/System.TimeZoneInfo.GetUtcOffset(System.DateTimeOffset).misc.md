---
uid: System.TimeZoneInfo.GetUtcOffset(System.DateTimeOffset)
additional_notes.usage: *content
---

<p>On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, this method applies only the current adjustment rule when calculating the offset from UTC if the current instance is <xref href="System.TimeZoneInfo.Local"></xref>. As a result, the method may not accurately calculate the difference between the local time and UTC on <code>dateTimeOffset</code>. For more information, see the Notes for Callers section in the <xref href="System.TimeZoneInfo.Local"></xref> property.</p>


