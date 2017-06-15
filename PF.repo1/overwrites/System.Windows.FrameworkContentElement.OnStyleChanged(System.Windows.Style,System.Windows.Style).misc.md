---
uid: System.Windows.FrameworkContentElement.OnStyleChanged(System.Windows.Style,System.Windows.Style)
additional_notes.overrides: *content
---

<p>Always call the base implementation, otherwise styles cannot be applied. Scenarios for overriding this method might include if your derived class has a specialized style selector, or caches style values. Theme changes will potentially invoke this method.</p>


