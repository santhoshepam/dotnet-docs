---
uid: System.TimeZone.ToLocalTime(System.DateTime)
additional_notes.overrides: *content
---

<p>Although it is not required, in most cases derived classes running under the .NET Framework version 2.0 should override the default implementation of this method. In the .NET Framework versions 1.0 and 1.1, the `ToLocalTime` method called the <xref href="System.TimeZone.GetUtcOffset(System.DateTime)"></xref> method and adjusted for daylight saving time when returning the local time. However, starting with the .NET Framework 2.0, the behavior of the default implementation depends on the <xref href="System.DateTime.Kind"></xref> property of the <code>time</code> parameter. If its value is <xref href="System.DateTimeKind.Local"></xref>, this method returns <code>time</code> unchanged. If its value is either <xref href="System.DateTimeKind.Utc"></xref> or <xref href="System.DateTimeKind.Unspecified"></xref>, this method assumes <code>time</code> is UTC and converts it to the local system time without calling the <xref href="System.TimeZone.GetUtcOffset(System.DateTime)"></xref> method.  
  
 The following code provides a simple override of the default implementation of the `ToLocalTime` method. In this code, the `internalTimeZone` variable represents a private instance of the `TimeZone` class:  
  
 [!code-csharp[System.TimeZone.ToLocalTime#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.TimeZone.ToLocalTime/CS/TimeZone_ToLocalTime.cs#1)]
 [!code-vb[System.TimeZone.ToLocalTime#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.TimeZone.ToLocalTime/VB/TimeZone_ToLocalTime.vb#1)]</p>


