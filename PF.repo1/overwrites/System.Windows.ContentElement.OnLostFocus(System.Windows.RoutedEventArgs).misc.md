---
uid: System.Windows.ContentElement.OnLostFocus(System.Windows.RoutedEventArgs)
additional_notes.overrides: *content
---

<p>Unless you have a deliberate and unusual need to not raise the focus events, make sure that your implementation calls the base implementation. Otherwise, the <xref href="System.Windows.ContentElement.LostFocus"></xref> event is not raised during typical user operations that ordinarily set focus to this element. If you do not intend your element to be focusable, you can prevent the element from being focusable by setting <xref href="System.Windows.ContentElement.Focusable"></xref> to `false`.</p>


