---
uid: System.DateTime.ToString
additional_notes.usage: *content
---

<p>The <xref href="System.DateTime.ToString"></xref> method returns the string representation of the date and time in the calendar used by the current culture. If the value of the current <xref href="System.DateTime"></xref> instance is earlier than <xref href="System.Globalization.Calendar.MinSupportedDateTime"></xref> or later than <xref href="System.Globalization.Calendar.MaxSupportedDateTime"></xref>, the method throws an <xref href="System.ArgumentOutOfRangeException"></xref>. The following example provides an illustration. It attempts to format a date that is outside the range of the <xref href="System.Globalization.HijriCalendar"></xref> class when the current culture is Arabic (Syria).  
  
 [!code-csharp[System.DateTime.ToString.ArgumentOutOfRangeException#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.datetime.tostring.argumentoutofrangeexception/cs/datetime.tostring.argumentoutofrangeexception2.cs#2)]
 [!code-vb[System.DateTime.ToString.ArgumentOutOfRangeException#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.datetime.tostring.argumentoutofrangeexception/vb/datetime.tostring.argumentoutofrangeexception2.vb#2)]</p>


