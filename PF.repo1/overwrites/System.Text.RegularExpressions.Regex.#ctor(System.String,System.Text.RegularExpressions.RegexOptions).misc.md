---
uid: System.Text.RegularExpressions.Regex.#ctor(System.String,System.Text.RegularExpressions.RegexOptions)
additional_notes.usage: *content
---

<p>This constructor creates a <xref href="System.Text.RegularExpressions.Regex"></xref> object that uses the default time-out value of the application domain in which it is created. If a time-out value has not been defined for the application domain, the <xref href="System.Text.RegularExpressions.Regex"></xref> object uses the value <xref href="System.Text.RegularExpressions.Regex.InfiniteMatchTimeout"></xref>, which prevents the operation from timing out. The recommended constructor for creating a <xref href="System.Text.RegularExpressions.Regex"></xref> object is <xref href="System.Text.RegularExpressions.Regex.#ctor(System.String,System.Text.RegularExpressions.RegexOptions,System.TimeSpan)"></xref>, which lets you set the time-out interval.</p>


