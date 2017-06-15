---
uid: System.Windows.FrameworkContentElement.BeginInit
additional_notes.overrides: *content
---

<p>Override this method to provide special handling that should occur before your element is initialized during the element loading process.  
  
 Your implementation should call the base implementation, because the base (default) implementation sets some internal flags to keep track of initialization.  
  
 The base implementation will throw an exception if <xref href="System.Windows.FrameworkContentElement.BeginInit"></xref> is called more than one time on the same element prior to reaching <xref href="System.Windows.FrameworkContentElement.EndInit"></xref>.</p>


