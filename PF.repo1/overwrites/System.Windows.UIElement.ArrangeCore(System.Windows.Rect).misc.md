---
uid: System.Windows.UIElement.ArrangeCore(System.Windows.Rect)
additional_notes.overrides: *content
---

<p>If you are developing elements at the WPF core level,you should override this method to give your WPF core-level element a unique arrange layout behavior, or to make proper layout decisions about the child elements of your elements. An override might be necessary if those child elements are not recognizable from a defined pattern such as an <xref href="System.Windows.Controls.ItemCollection"></xref>.  
  
 A parent element must call the class-specific <xref href="System.Windows.UIElement.Arrange(System.Windows.Rect)"></xref> on each child element, otherwise those child elements are not rendered.</p>


