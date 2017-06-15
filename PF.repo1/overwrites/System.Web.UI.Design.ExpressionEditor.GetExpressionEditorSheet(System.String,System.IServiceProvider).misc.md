---
uid: System.Web.UI.Design.ExpressionEditor.GetExpressionEditorSheet(System.String,System.IServiceProvider)
additional_notes.overrides: *content
---

<p>Typically, to supply a new expression type at design time, you define a unique expression prefix and provide custom <xref href="System.Web.Compilation.ExpressionBuilder"></xref> and <xref href="System.Web.UI.Design.ExpressionEditor"></xref> implementations. Optionally, you can provide a custom <xref href="System.Web.UI.Design.ExpressionEditorSheet"></xref> implementation that defines properties that are used to form the expression. Even though the configuration file defines the prefix, you should also apply an <xref href="System.Web.Compilation.ExpressionPrefixAttribute"></xref> object and an <xref href="System.Web.Compilation.ExpressionEditorAttribute"></xref> object.  
  
 Override the <xref href="System.Web.UI.Design.ExpressionEditor.GetExpressionEditorSheet(System.String,System.IServiceProvider)"></xref> method to return an expression editor sheet that defines design-time input for multiple properties in a custom expression. When you select a control property and the expression editor type, the visual designer calls the <xref href="System.Web.UI.Design.ExpressionEditor.GetExpressionEditorSheet(System.String,System.IServiceProvider)"></xref> method, and then supplies the current expression string that is set for the control property. Use <code>expression</code> to set the initial values for the expression properties. Use <code>serviceProvider</code> to initialize a custom expression sheet constructor and to access services that are provided by the designer host. For example, call the <xref href="System.IServiceProvider.GetService(System.Type)"></xref> method with the <xref href="System.Web.UI.Design.IWebApplication"></xref> type to access project items, documents, or configuration file details that are provided through the visual designer.</p>


