---
uid: System.DateTimeOffset.ToString(System.String,System.IFormatProvider)
additional_notes.usage: *content
---

<p>The <xref href="System.DateTimeOffset.ToString(System.String,System.IFormatProvider)"></xref> method returns the string representation of the date and time in the calendar used by the <code>formatProvider</code> parameter. Its calendar is defined by the <xref href="System.Globalization.DateTimeFormatInfo.Calendar"></xref> property. If the value of the current <xref href="System.DateTimeOffset"></xref> instance is earlier than <xref href="System.Globalization.Calendar.MinSupportedDateTime"></xref> or later than <xref href="System.Globalization.Calendar.MaxSupportedDateTime"></xref>, the method throws an <xref href="System.ArgumentOutOfRangeException"></xref>. The following example provides an illustration. It attempts to format a date that is outside the range of the <xref href="System.Globalization.UmAlQuraCalendar"></xref> class.  
  
 [!code-csharp[System.DateTimeOffset.ToString.ArgumentOutOfRangeException#4](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.datetimeoffset.tostring.argumentoutofrangeexception/cs/datetimeoffset.tostring.argumentoutofrangeexception4.cs#4)]
 [!code-vb[System.DateTimeOffset.ToString.ArgumentOutOfRangeException#4](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.datetimeoffset.tostring.argumentoutofrangeexception/vb/datetimeoffset.tostring.argumentoutofrangeexception4.vb#4)]</p>


