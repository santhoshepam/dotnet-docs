---
uid: System.DateTime.ToLocalTime
additional_notes.usage: *content
---

<p>You can use the <xref href="System.DateTime.ToLocalTime"></xref> method to restore a local date and time value that was converted to UTC by the <xref href="System.DateTime.ToUniversalTime"></xref> or <xref href="System.DateTime.FromFileTimeUtc(System.Int64)"></xref> method. However, if the original time represents an invalid time in the local time zone, it will not match the restored value. When the <xref href="System.DateTime.ToLocalTime"></xref> method converts a time from UTC to the local time zone, it also adjusts the time so that is valid in the local time zone.  
  
 For example, the transition from standard time to daylight saving time occurs in the U.S. Pacific Time zone on March 14, 2010, at 2:00 A.M., when the time advances by one hour, to 3:00 A.M. This hour interval is an invalid time, that is, a time interval that does not exist in this time zone. The following example shows that when a time that falls within this range is converted to UTC by the <xref href="System.DateTime.ToUniversalTime"></xref> method and is then restored by the <xref href="System.DateTime.ToLocalTime"></xref> method, the original value is adjusted to become a valid time. You can determine whether a particular date and time value may be subject to modification by passing it to the <xref href="System.TimeZoneInfo.IsInvalidTime(System.DateTime)"></xref> method, as the example illustrates.  
  
 [!code-csharp[System.DateTime.ToLocalTime#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.datetime.tolocaltime/cs/tolocaltime1.cs#1)]
 [!code-vb[System.DateTime.ToLocalTime#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.datetime.tolocaltime/vb/tolocaltime1.vb#1)]</p>


