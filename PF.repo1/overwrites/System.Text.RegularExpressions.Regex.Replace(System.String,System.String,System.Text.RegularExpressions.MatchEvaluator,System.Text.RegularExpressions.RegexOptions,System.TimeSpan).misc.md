---
uid: System.Text.RegularExpressions.Regex.Replace(System.String,System.String,System.Text.RegularExpressions.MatchEvaluator,System.Text.RegularExpressions.RegexOptions,System.TimeSpan)
additional_notes.usage: *content
---

<p>We recommend that you set the <code>matchTimeout</code> parameter to an appropriate value, such as two seconds. If you disable time-outs by specifying <xref href="System.Text.RegularExpressions.Regex.InfiniteMatchTimeout"></xref>, the regular expression engine offers slightly better performance. However, you should disable time-outs only under the following conditions:  
  
-   When the input processed by a regular expression is derived from a known and trusted source or consists of static text. This excludes text that has been dynamically input by users.  
  
-   When the regular expression pattern has been thoroughly tested to ensure that it efficiently handles matches, non-matches, and near matches.  
  
-   When the regular expression pattern contains no language elements that are known to cause excessive backtracking when processing a near match.</p>


