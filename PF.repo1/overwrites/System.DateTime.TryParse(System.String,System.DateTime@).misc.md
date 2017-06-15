---
uid: System.DateTime.TryParse(System.String,System.DateTime@)
additional_notes.usage: *content
---

<p>Formatting is influenced by properties of the current <xref href="System.Globalization.DateTimeFormatInfo"></xref> object, which by default are derived from the **Regional and Language Options** item in Control Panel. The <xref href="System.DateTime.TryParse*"></xref> method can unexpectedly fail and return `False` if the current <xref href="System.Globalization.DateTimeFormatInfo.DateSeparator"></xref> and <xref href="System.Globalization.DateTimeFormatInfo.TimeSeparator"></xref> properties are set to the same value.</p>


