---
uid: System.Web.UI.Design.ExpressionEditor
additional_notes.overrides: *content
---

<p>The following steps are required in deriving a custom <xref href="System.Web.UI.Design.ExpressionEditor"></xref> class:  
  
-   Override the <xref href="System.Web.UI.Design.ExpressionEditor.EvaluateExpression(System.String,System.Object,System.Type,System.IServiceProvider)"></xref> method to evaluate the custom expression type at design time.  
  
-   Optionally, override the <xref href="System.Web.UI.Design.ExpressionEditor.GetExpressionEditorSheet(System.String,System.IServiceProvider)"></xref> method to return a custom class that defines properties that are combined to form the custom expression.  
  
-   Apply the <xref href="System.Web.Compilation.ExpressionEditorAttribute"></xref> attribute on the <xref href="System.Web.Compilation.ExpressionBuilder"></xref> class declaration to associate the custom expression builder with the derived expression editor class.  
  
 For example, the <xref href="System.Web.UI.Design.ResourceExpressionEditor"></xref> class derives from the <xref href="System.Web.UI.Design.ExpressionEditor"></xref> class and provides an implementation for evaluating and associating a resource string reference with a control property at design time. The <xref href="System.Web.Compilation.ResourceExpressionBuilder"></xref> class is associated with the expression prefix `Resources` and the <xref href="System.Web.UI.Design.ResourceExpressionEditor"></xref> implementation. The <xref href="System.Web.UI.Design.ResourceExpressionEditor.GetExpressionEditorSheet(System.String,System.IServiceProvider)"></xref> method returns a <xref href="System.Web.UI.Design.ResourceExpressionEditorSheet"></xref>, which defines the individual properties that form a resource reference expression.</p>


