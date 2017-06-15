---
uid: System.IConvertible
additional_notes.overrides: *content
---

<p>If you implement the <xref href="System.IConvertible"></xref> interface, your implementation will be called automatically by the <xref href="System.Convert.ChangeType(System.Object,System.Type)"></xref> method if the <xref href="System.Object"></xref> parameter is an instance of your implementing type and the <xref href="System.Type"></xref> parameter is a common language runtime type.  
  
 Most conversion methods have a parameter of type <xref href="System.IFormatProvider"></xref> that represents either the current culture (<xref href="System.Globalization.CultureInfo.CurrentCulture"></xref>) or a specific culture. For the most part, the <xref href="System.IConvertible"></xref> implementations of the base types ignore this parameter. However, you can choose whether to use it in your code.</p>


