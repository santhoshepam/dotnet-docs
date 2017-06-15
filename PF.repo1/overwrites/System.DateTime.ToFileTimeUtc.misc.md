---
uid: System.DateTime.ToFileTimeUtc
additional_notes.usage: *content
---

<p>The <xref href="System.DateTime.ToFileTimeUtc"></xref> method is sometimes used to convert a local time to UTC, and subsequently to restore it by calling the <xref href="System.DateTime.FromFileTimeUtc(System.Int64)"></xref> method followed by the <xref href="System.DateTime.ToLocalTime"></xref> method. However, if the original time represents an invalid time in the local time zone, the two local time values will not be equal. For additional information, see the <xref href="System.DateTime.ToLocalTime"></xref> method.</p>


