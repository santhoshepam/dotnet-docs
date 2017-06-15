---
uid: System.Collections.Generic.Comparer`1
additional_notes.overrides: *content
---

<p>
      <xref href="System.Collections.Generic.Comparer`1.Compare(`0,`0)"></xref> and <xref href="System.Collections.Generic.EqualityComparer`1.Equals(`0,`0)"></xref> may behave differently in terms of culture-sensitivity and case-sensitivity.  
  
 For string comparisons, the <xref href="System.StringComparer"></xref> class is recommended over <code>Comparer<String></code>.  Properties of the <xref href="System.StringComparer"></xref> class return predefined instances that perform string comparisons with different combinations of culture-sensitivity and case-sensitivity.  The case-sensitivity and culture-sensitivity are consistent among the members of the same <xref href="System.StringComparer"></xref> instance.  
  
 For more information on culture-specific comparisons, see the <xref href="System.Globalization"></xref> namespace and [Globalization and Localization](http://msdn.microsoft.com/library/9a59696b-d89b-45bd-946d-c75da4732d02).</p>


