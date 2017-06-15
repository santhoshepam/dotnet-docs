---
uid: System.Windows.RoutedEventArgs.InvokeEventHandler(System.Delegate,System.Object)
additional_notes.overrides: *content
---

<p>This method is intended to be overridden by derived event data classes to provide more efficient invocation of their delegates. The implementation should cast the provided <code>genericHandler</code> to the type-specific delegate, and then invoke that handler.  
  
 The default implementation will attempt to invoke the provided handler, attempting to cast it as <xref href="System.Windows.RoutedEventHandler"></xref>. If either <code>genericHandler</code> or <code>genericTarget</code> is provided as `null`, exceptions will be raised.</p>


