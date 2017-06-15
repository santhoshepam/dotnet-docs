---
uid: System.Char.ToLower(System.Char)
additional_notes.usage: *content
---

<p>As explained in [Best Practices for Using Strings](~/docs/standard/base-types/best-practices-strings.md), we recommend that you avoid calling character-casing and string-casing methods that substitute default values. Instead, you should call methods that require parameters to be explicitly specified. To convert a character to lowercase by using the casing conventions of the current culture, call the <xref href="System.Char.ToLower(System.Char,System.Globalization.CultureInfo)"></xref> method overload with a value of <xref href="System.Globalization.CultureInfo.CurrentCulture"></xref> for its <code>culture</code> parameter.</p>


