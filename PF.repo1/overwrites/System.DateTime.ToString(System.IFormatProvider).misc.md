---
uid: System.DateTime.ToString(System.IFormatProvider)
additional_notes.usage: *content
---

<p>The <xref href="System.DateTime.ToString(System.IFormatProvider)"></xref> method returns the string representation of the date and time in the calendar used by the culture represented by the <code>provider</code> parameter. Its calendar is defined by the <xref href="System.Globalization.DateTimeFormatInfo.Calendar"></xref> property. If the value of the current <xref href="System.DateTime"></xref> instance is earlier than <xref href="System.Globalization.Calendar.MinSupportedDateTime"></xref> or later than <xref href="System.Globalization.Calendar.MaxSupportedDateTime"></xref>, the method throws an <xref href="System.ArgumentOutOfRangeException"></xref>. The following example provides an illustration. It attempts to format a date that is outside the range of the <xref href="System.Globalization.JapaneseCalendar"></xref> class.  
  
 [!code-csharp[System.DateTime.ToString.ArgumentOutOfRangeException#1](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.datetime.tostring.argumentoutofrangeexception/cs/datetime.tostring.argumentoutofrangeexception1.cs#1)]
 [!code-vb[System.DateTime.ToString.ArgumentOutOfRangeException#1](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.datetime.tostring.argumentoutofrangeexception/vb/datetime.tostring.argumentoutofrangeexception1.vb#1)]</p>


