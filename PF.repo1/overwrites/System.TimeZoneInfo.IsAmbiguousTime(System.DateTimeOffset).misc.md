---
uid: System.TimeZoneInfo.IsAmbiguousTime(System.DateTimeOffset)
additional_notes.usage: *content
---

<p>On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, this method applies only the current adjustment rule if the current instance is <xref href="System.TimeZoneInfo.Local"></xref>. As a result, the method may not accurately report whether <code>dateTimeOffset</code> is an ambiguous time for periods before the current adjustment rule came into effect. For more information, see the Notes for Callers section in the <xref href="System.TimeZoneInfo.Local"></xref> property.</p>


