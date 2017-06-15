---
uid: System.DateTime.ToFileTime
additional_notes.usage: *content
---

<p>Ordinarily, the <xref href="System.DateTime.FromFileTime(System.Int64)"></xref> method restores a <xref href="System.DateTime"></xref> value that was saved by the <xref href="System.DateTime.ToFileTime"></xref> method. However, the two values may differ under the following conditions:  
  
-   If the serialization and deserialization of the <xref href="System.DateTime"></xref> value occur in different time zones. For example, if a <xref href="System.DateTime"></xref> value with a time of 12:30 P.M. in the U.S. Eastern Time zone is serialized, and then deserialized in the U.S. Pacific Time zone, the original value of 12:30 P.M. is adjusted to 9:30 A.M. to reflect the difference between the two time zones.  
  
-   If the <xref href="System.DateTime"></xref> value that is serialized represents an invalid time in the local time zone. In this case, the <xref href="System.DateTime.ToFileTime"></xref> method adjusts the restored <xref href="System.DateTime"></xref> value so that it represents a valid time in the local time zone.  
  
     For example, the transition from standard time to daylight saving time occurs in the U.S. Pacific Time zone on March 14, 2010, at 2:00 A.M., when the time advances by one hour, to 3:00 A.M. This hour interval is an invalid time, that is, a time interval that does not exist in this time zone. The following example shows that when a time that falls within this range is converted to a long integer value by the <xref href="System.DateTime.ToFileTime"></xref> method and is then restored by the <xref href="System.DateTime.FromFileTime(System.Int64)"></xref> method, the original value is adjusted to become a valid time. You can determine whether a particular date and time value may be subject to modification by passing it to the <xref href="System.TimeZoneInfo.IsInvalidTime(System.DateTime)"></xref> method, as the example illustrates.  
  
     [!code-csharp[System.DateTime.FromFileTime#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.datetime.fromfiletime/cs/fromfiletime1.cs#1)]
     [!code-vb[System.DateTime.FromFileTime#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.datetime.fromfiletime/vb/fromfiletime1.vb#1)]</p>


