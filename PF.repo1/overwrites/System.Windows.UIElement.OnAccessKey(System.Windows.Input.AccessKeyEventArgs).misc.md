---
uid: System.Windows.UIElement.OnAccessKey(System.Windows.Input.AccessKeyEventArgs)
additional_notes.overrides: *content
---

<p>The default implementation of this method in <xref href="System.Windows.UIElement"></xref> sets keyboard focus to this element (by calling <xref href="System.Windows.UIElement.Focus"></xref>). Implementations should perpetuate this behavior if they are focusable, because it is an expected behavior for accessibility scenarios. Note that the base implementation does nothing with the passed event data and raises no further event; it just sets the focus.</p>


