---
uid: System.Windows.UIElement.IsEnabledCore
additional_notes.overrides: *content
---

<p>The default implementation of this property caches the value and also calculates whether the parent element of this element is enabled. (If the parent is not enabled, the child element cannot be effectively enabled in practical [!INCLUDE[TLA#tla_ui](~/includes/tlasharptla-ui-md.md)].) If you choose to override this implementation, make certain that you call the base implementation to preserve this behavior.  
  
 The <xref href="System.Windows.Controls.Primitives.ScrollBar"></xref> class provides an existing override implementation of this property. This override determines whether the content inside the content presentation area exceeds the available area. If the content does exceed the area, the scrollbar portion is enabled. Otherwise, the scrollbar is not enabled.</p>


