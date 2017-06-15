---
uid: System.Object.ToString
additional_notes.overrides: *content
---

<p>When you implement your own types, you should override the <xref href="System.Object.ToString"></xref> method to return values that are meaningful for those types. Derived classes that require more control over formatting than <xref href="System.Object.ToString"></xref> provides can implement the <xref href="System.IFormattable"></xref> interface. Its <xref href="System.IFormattable.ToString(System.String,System.IFormatProvider)"></xref> method enables you to define format strings that control formatting and to use an <xref href="System.IFormatProvider"></xref> object that can provide for culture-specific formatting.  
  
 Overrides of the <xref href="System.Object.ToString"></xref> method should follow these guidelines:  
  
-   The returned string should be friendly and readable by humans.  
  
-   The returned string should uniquely identify the value of the object instance.  
  
-   The returned string should be as short as possible so that it is suitable for display by a debugger.  
  
-   Your <xref href="System.Object.ToString"></xref> override should not return <xref href="System.String.Empty"></xref> or a null string.  
  
-   Your <xref href="System.Object.ToString"></xref> override should not throw an exception.  
  
-   If the string representation of an instance is culture-sensitive or can be formatted in multiple ways, implement the <xref href="System.IFormattable"></xref> interface.  
  
-   If the returned string includes sensitive information, you should first demand an appropriate permission. If the demand succeeds, you can return the sensitive information; otherwise, you should return a string that excludes the sensitive information.  
  
-   Your <xref href="System.Object.ToString"></xref> override should have no observable side effects to avoid complications in debugging. For example, a call to the <xref href="System.Object.ToString"></xref> method should not change the value of instance fields.  
  
-   If your type implements a parsing method (or `Parse` or `TryParse` method, a constructor, or some other static method that instantiates an instance of the type from a string), you should ensure that the string returned by the <xref href="System.Object.ToString"></xref> method can be converted to an object instance.</p>


