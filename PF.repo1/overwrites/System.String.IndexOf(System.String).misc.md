---
uid: System.String.IndexOf(System.String)
additional_notes.usage: *content
---

<p>As explained in [Best Practices for Using Strings](~/docs/standard/base-types/best-practices-strings.md), we recommend that you avoid calling string comparison methods that substitute default values and instead call methods that require parameters to be explicitly specified. To find the first index of a substring within a string instance by using the comparison rules of the current culture, call the <xref href="System.String.IndexOf(System.String,System.StringComparison)"></xref> method overload with a value of <xref href="System.StringComparison.CurrentCulture"></xref> for its <code>comparisonType</code> parameter.</p>


