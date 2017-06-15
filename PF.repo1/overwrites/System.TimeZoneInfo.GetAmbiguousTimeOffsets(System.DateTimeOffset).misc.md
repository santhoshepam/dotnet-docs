---
uid: System.TimeZoneInfo.GetAmbiguousTimeOffsets(System.DateTimeOffset)
additional_notes.usage: *content
---

<p>On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, this method applies only the current adjustment rule when determining whether <code>dateTimeOffset</code> is ambiguous if the current instance is <xref href="System.TimeZoneInfo.Local"></xref>. As a result, the method may not accurately report ambiguous time offsets for periods before the current adjustment rule came into effect. For more information, see the Notes for Callers section in the <xref href="System.TimeZoneInfo.Local"></xref> property.</p>


