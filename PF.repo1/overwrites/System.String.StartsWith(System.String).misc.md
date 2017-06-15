---
uid: System.String.StartsWith(System.String)
additional_notes.usage: *content
---

<p>As explained in [Best Practices for Using Strings](~/docs/standard/base-types/best-practices-strings.md), we recommend that you avoid calling string comparison methods that substitute default values and instead call methods that require parameters to be explicitly specified. To determine whether a string begins with a particular substring by using the string comparison rules of the current culture, call the <xref href="System.String.StartsWith(System.String,System.StringComparison)"></xref> method overload with a value of <xref href="System.StringComparison.CurrentCulture"></xref> for its <code>comparisonType</code> parameter.</p>


