---
uid: System.Windows.UIElement3D.IsEnabledCore
additional_notes.overrides: *content
---

<p>The default implementation of this property caches the value and also calculates whether the parent element of this element is enabled. (If the parent is not enabled, the child element cannot be effectively enabled in practical [!INCLUDE[TLA#tla_ui](~/includes/tlasharptla-ui-md.md)].) If you choose to override this implementation, make certain that you call the base implementation to preserve this behavior.</p>


