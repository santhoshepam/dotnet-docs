---
uid: System.TimeZoneInfo.IsInvalidTime(System.DateTime)
additional_notes.usage: *content
---

<p>On [!INCLUDE[winxp](~/includes/winxp-md.md)] systems, this method applies only the adjustment rule if the current instance is <xref href="System.TimeZoneInfo.Local"></xref>. As a result, the method may not accurately report whether <code>dateTime</code> is an invalid time for periods before the current adjustment rule came into effect. For more information, see the Notes for Callers section in the <xref href="System.TimeZoneInfo.Local"></xref> property.</p>


