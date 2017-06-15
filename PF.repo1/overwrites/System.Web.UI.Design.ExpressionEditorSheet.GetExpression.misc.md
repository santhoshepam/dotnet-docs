---
uid: System.Web.UI.Design.ExpressionEditorSheet.GetExpression
additional_notes.overrides: *content
---

<p>Derive a custom expression editor sheet from the <xref href="System.Web.UI.Design.ExpressionEditorSheet"></xref> class, if you are defining a new expression type for control property values and you want to build the expression string based on multiple expression property values. A derived class implementation should contain the following:  
  
-   A public property for each distinct value in the expression string that can be set at design time.  
  
-   An implementation of the <xref href="System.Web.UI.Design.ExpressionEditorSheet.GetExpression"></xref> method that forms the custom expression string from the editor sheet property values.  
  
-   Optionally, a constructor implementation that sets the initial values of the editor sheet properties.  
  
 The associated custom expression editor class creates an instance of the derived editor sheet in the <xref href="System.Web.UI.Design.ExpressionEditor.GetExpressionEditorSheet(System.String,System.IServiceProvider)"></xref> method, initializes that instance with the current expression string set for the control property, and then returns the instance to the visual designer. The visual designer allows you to set the expression sheet properties, and then calls the <xref href="System.Web.UI.Design.ExpressionEditorSheet.GetExpression"></xref> method to form the expression string from the input expression sheet property values.</p>


