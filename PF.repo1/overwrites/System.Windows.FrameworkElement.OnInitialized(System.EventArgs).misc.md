---
uid: System.Windows.FrameworkElement.OnInitialized(System.EventArgs)
additional_notes.overrides: *content
---

<p>The default implementation of this virtual method raises the event as described above. Overrides should call the base implementation to preserve this behavior. If you fail to call the base implementation, not only will you not raise the <xref href="System.Windows.FrameworkElement.Initialized"></xref> event as is generally expected of a <xref href="System.Windows.FrameworkElement"></xref> derived class, but you will also suppress two important style and theme style initialization operations that are implemented by this base implementation.</p>


