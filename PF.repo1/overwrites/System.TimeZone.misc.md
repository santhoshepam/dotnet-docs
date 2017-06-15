---
uid: System.TimeZone
additional_notes.overrides: *content
---

<p>In addition to providing implementations for its `abstract` members (those marked `MustOverride` in Visual Basic), it is important that classes derived from <xref href="System.TimeZone"></xref> override the default behavior of the <xref href="System.TimeZone.ToLocalTime(System.DateTime)"></xref> method. This is because the default behavior of <xref href="System.TimeZone.ToLocalTime(System.DateTime)"></xref> in the .NET Framework version 2.0 does not depend on a call to <xref href="System.TimeZone.GetUtcOffset(System.DateTime)"></xref>, as it did in the .NET Framework versions 1.0 and 1.1.  For details, see the <xref href="System.TimeZone.ToLocalTime(System.DateTime)"></xref> method.</p>


