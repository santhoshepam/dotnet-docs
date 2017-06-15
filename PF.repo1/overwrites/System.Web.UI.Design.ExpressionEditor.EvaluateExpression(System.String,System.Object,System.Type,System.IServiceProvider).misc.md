---
uid: System.Web.UI.Design.ExpressionEditor.EvaluateExpression(System.String,System.Object,System.Type,System.IServiceProvider)
additional_notes.overrides: *content
---

<p>Classes deriving from the <xref href="System.Web.UI.Design.ExpressionEditor"></xref> class must override the <xref href="System.Web.UI.Design.ExpressionEditor.EvaluateExpression(System.String,System.Object,System.Type,System.IServiceProvider)"></xref> method to evaluate the custom expression type at design time.  
  
 At a minimum, an <xref href="System.Web.UI.Design.ExpressionEditor.EvaluateExpression(System.String,System.Object,System.Type,System.IServiceProvider)"></xref> implementation must use the following steps:  
  
1.  Evaluate the expression string and determine the object that is referenced by the expression.  
  
2.  Return `null`, if the expression string cannot be evaluated.  
  
3.  Use the <xref href="System.Type.IsAssignableFrom(System.Type)"></xref> method on <code>propertyType</code> to determine whether the referenced object can be assigned directly to the control property type, and then, depending on the result, complete one of the following actions:  
  
    -   If the referenced object can be assigned directly to the control property, return the referenced object for the expression.  
  
    -   If the referenced object is a simple type, such as a string, return the referenced object.  
  
    -   Otherwise, determine whether the referenced object can be assigned to or converted to the property type.  
  
4.  Use the <xref href="System.ComponentModel.TypeConverter.CanConvertFrom*"></xref> method on the <xref href="System.ComponentModel.TypeConverter"></xref> object for <code>propertyType</code> to determine whether the referenced object can be converted to the control property type, and then, depending on the result, complete one of the following actions:  
  
    -   If the object can be converted to the control property type, return the converted object using the <xref href="System.ComponentModel.TypeConverter.ConvertFrom*"></xref> method.  
  
    -   If the referenced object cannot be assigned or converted to <code>propertyType</code>, return the referenced object.  
  
 Optionally, the <xref href="System.Web.UI.Design.ExpressionEditor.EvaluateExpression(System.String,System.Object,System.Type,System.IServiceProvider)"></xref> implementation can use the <code>parseTimeData</code> object that is supplied by the <xref href="System.Web.Compilation.ExpressionBuilder.ParseExpression(System.String,System.Type,System.Web.Compilation.ExpressionBuilderContext)"></xref> implementation to optimize or help in the evaluation of the input expression string.</p>


