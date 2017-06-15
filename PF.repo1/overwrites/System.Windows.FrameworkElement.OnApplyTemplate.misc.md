---
uid: System.Windows.FrameworkElement.OnApplyTemplate
additional_notes.overrides: *content
---

<p>Derived classes of <xref href="System.Windows.FrameworkElement"></xref> can use this method as a notification for a variety of possible scenarios:  
  
-   You can call your own implementation of code that builds the remainder of an element visual tree.  
  
-   You can run code that relies on the visual tree from templates having been applied, such as obtaining references to named elements that came from a template.  
  
-   You can introduce services that only make sense to exist after the visual tree from templates is complete.  
  
-   You can set states and properties of elements within the template that are dependent on other factors. For instance, property values might only be discoverable by knowing the parent element, or when a specific derived class uses a common template.  
  
 Implementers should always call the base implementation before their own implementation. <xref href="System.Windows.FrameworkElement"></xref> itself has no default implementation, but intervening classes might.  
  
 <xref href="System.Windows.Controls.Control"></xref> offers a similar override, <xref href="System.Windows.Controls.Control.OnTemplateChanged(System.Windows.Controls.ControlTemplate,System.Windows.Controls.ControlTemplate)"></xref>.</p>


