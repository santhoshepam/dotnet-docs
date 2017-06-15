---
uid: System.TimeZone.CurrentTimeZone
additional_notes.usage: *content
---

<p>Local time zone data is cached after <xref href="System.TimeZone.CurrentTimeZone"></xref> is first used to retrieve time zone information. If the system's local time zone subsequently changes, the <xref href="System.TimeZone.CurrentTimeZone"></xref> property does not reflect this change. If you need to handle time zone changes while your application is running, use the <xref href="System.TimeZoneInfo"></xref> class and call its <xref href="System.TimeZoneInfo.ClearCachedData"></xref> method.</p>


