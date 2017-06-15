---
uid: System.Windows.FrameworkElement.BeginInit
additional_notes.overrides: *content
---

<p>Implement this method to provide special handling that should happen before your element is initialized during the element loading process.  
  
 Your implementation should call the base implementation, because the base (default) implementation sets some internal flags to keep track of initialization. One possible implementation is to use this method as a hook into your own private class initialization routines that are not already enabled by constructors.  
  
 The base implementation will throw an exception if <xref href="System.Windows.FrameworkElement.BeginInit"></xref> is called more than one time on the same element prior to <xref href="System.Windows.FrameworkElement.EndInit"></xref> being called.</p>


