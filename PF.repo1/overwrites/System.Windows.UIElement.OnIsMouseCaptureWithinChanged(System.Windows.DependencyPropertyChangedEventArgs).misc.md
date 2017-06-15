---
uid: System.Windows.UIElement.OnIsMouseCaptureWithinChanged(System.Windows.DependencyPropertyChangedEventArgs)
additional_notes.overrides: *content
---

<p>This virtual method is raised when the value of the <xref href="System.Windows.UIElement.IsMouseCaptureWithin"></xref> dependency property changes its value. The virtual method is raised first and can manipulate the event data as necessary. Then the <xref href="System.Windows.UIElement.IsMouseCaptureWithinChanged"></xref> event is raised with that same event data instance. Notice that the event is not a routed event; Therefore,  you cannot mark it as handled in the class handler.  
  
 This method has no default implementation. Because an intermediate class in the inheritance might implement this method, we recommend that you call the base implementation in your implementation. You may call base either before or after your special handling, depending on your requirements.</p>


