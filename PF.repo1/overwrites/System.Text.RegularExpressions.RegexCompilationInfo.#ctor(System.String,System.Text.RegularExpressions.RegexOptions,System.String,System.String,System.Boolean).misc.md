---
uid: System.Text.RegularExpressions.RegexCompilationInfo.#ctor(System.String,System.Text.RegularExpressions.RegexOptions,System.String,System.String,System.Boolean)
additional_notes.usage: *content
---

<p>This constructor creates a compiled regular expression that uses the default time-out value of the application domain in which it is created. If a time-out value is defined for the application domain, the compiled regular expression uses the value <xref href="System.Text.RegularExpressions.Regex.InfiniteMatchTimeout"></xref>, which prevents a pattern-matching operation from timing out. The recommended constructor for creating a compiled regular expression is <xref href="System.Text.RegularExpressions.RegexCompilationInfo.#ctor(System.String,System.Text.RegularExpressions.RegexOptions,System.String,System.String,System.Boolean,System.TimeSpan)"></xref>, which lets you set the time-out interval.</p>


