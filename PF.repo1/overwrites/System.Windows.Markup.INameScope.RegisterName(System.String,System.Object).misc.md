---
uid: System.Windows.Markup.INameScope.RegisterName(System.String,System.Object)
additional_notes.overrides: *content
---

<p>Do not permit duplicate names to be registered. If the input <code>name</code> is already assigned to an existing element in the internal collection representation of the XAML namescope (even if it is the same as <code>scopedElement</code>), throw an exception.  
  
 Also consider throwing an exception if the provided name does not conform to [XamlName Grammar](~/docs/framework/xaml-services/xamlname-grammar.md).</p>


