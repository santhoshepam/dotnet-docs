---
uid: System.Windows.Forms.AccessibleObject.Navigate(System.Windows.Forms.AccessibleNavigation)
additional_notes.overrides: *content
---

<p>All visual objects must support this method. If an object has the state <xref href="System.Windows.Forms.AccessibleStates.Invisible"></xref>, navigation to this hidden object might fail. Some system-defined interface elements such as menus, menu items, and pop-up menus allow navigation to objects that are not visible. However, other system-defined user interface elements do not support this. If possible, servers should support navigation to objects that are not visible, but this support is not required and clients should not expect it.</p>


