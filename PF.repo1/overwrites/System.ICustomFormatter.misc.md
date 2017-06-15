---
uid: System.ICustomFormatter
additional_notes.overrides: *content
---

<p>The common language runtime attempts to use your <xref href="System.ICustomFormatter"></xref> implementation for every format item in a composite format string. As a result, you should expect that your <xref href="System.ICustomFormatter"></xref> implementation will be called to provide formatting services to objects or values that it is not designed to handle. In these cases, your <xref href="System.ICustomFormatter.Format(System.String,System.Object,System.IFormatProvider)"></xref> method must call the appropriate formatting method for that object or value.  
  
 There are two kinds of <xref href="System.ICustomFormatter"></xref> implementations: intrinsic and extension.  
  
 Intrinsic implementations are implementations that provide custom formatting for an application-defined object. In this case, your implementation should include the following:  
  
-   A definition of format strings that define the formatting of the object. Format strings are optional. Typically, a "G" or "g" format string defines the general (or most commonly used) format. However, you are free to define any format strings that you choose. You are also free to decide whether they are case-sensitive or case-insensitive.  
  
-   A test to ensure that the type of the object passed to your <xref href="System.ICustomFormatter.Format(System.String,System.Object,System.IFormatProvider)"></xref> method is your application-defined type. If it is not, you should call the object's <xref href="System.IFormattable"></xref> implementation, if one exists, or its <xref href="System.Object.ToString"></xref> method, if it does not. You should be prepared to handle any exceptions these method calls might throw.  
  
-   Code to handle a null format string, if your implementation supports format strings. The most common approach is to replace a null format string with the general format specifier.  
  
-   Code to handle any format strings that your implementation supports.  
  
-   Code to handle format strings that you do not support. The most common approach is to throw a <xref href="System.FormatException"></xref>, although you can provide default formatting.  
  
 Extension implementations are implementations that provide custom formatting for a type that already has formatting support. For example, you could define a <code>CustomerNumberFormatter</code> that formats an integral type with hyphens between specific digits. In this case, your implementation should include the following:  
  
-   A definition of format strings that extend the formatting of the object. These format strings are required, but they must not conflict with the type's existing format strings. For example, if you are extending formatting for the <xref href="System.Int32"></xref> type, you should not implement the "C", "D", "E", "F", and "G" format specifiers, among others.  
  
-   A test that the type of the object passed to your <xref href="System.ICustomFormatter.Format(System.String,System.Object,System.IFormatProvider)"></xref> method is a type whose formatting your extension supports. If it is not, call the object's <xref href="System.IFormattable"></xref> implementation, if one exists, or the object's parameterless <xref href="System.Object.ToString"></xref> method, if it does not. You should be prepared to handle any exceptions these method calls might throw.  
  
-   Code to handle any format strings that your extension supports.  
  
-   Code to handle any format strings that your extension does not support. These should be passed on to the type's <xref href="System.IFormattable"></xref> implementation. You should be prepared to handle any exceptions these method calls might throw.</p>


