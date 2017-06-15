---
uid: System.IFormattable
additional_notes.overrides: *content
---

<p>Classes that require more control over the formatting of strings than <xref href="System.Object.ToString"></xref> provides should implement <xref href="System.IFormattable"></xref>.  
  
 A class that implements <xref href="System.IFormattable"></xref> must support the "G" (general) format specifier. Besides the "G" specifier, the class can define the list of format specifiers that it supports. In addition, the class must be prepared to handle a format specifier that is `null`. For more information about formatting and formatting codes, see [Formatting Types](~/docs/standard/base-types/formatting-types.md)</p>


