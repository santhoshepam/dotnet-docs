---
uid: System.Windows.FrameworkPropertyMetadata.Merge(System.Windows.PropertyMetadata,System.Windows.DependencyProperty)
additional_notes.overrides: *content
---

<p>Classes that derive from <xref href="System.Windows.PropertyMetadata"></xref> (or this class particularly) should override this method to account for any metadata properties they have added in their implementations. For instance, your implementation might have added a new flagwise enumeration value, and the <xref href="System.Windows.FrameworkPropertyMetadata.Merge(System.Windows.PropertyMetadata,System.Windows.DependencyProperty)"></xref> implementation should then be able to combine those flags correctly.  
  
 Always call the base implementation prior to your own implementation, because the base implementation takes care of merging all the properties already defined on previous types in the hierarchy.  
  
 The behavior added by the <xref href="System.Windows.FrameworkPropertyMetadata.Merge(System.Windows.PropertyMetadata,System.Windows.DependencyProperty)"></xref> implementation in <xref href="System.Windows.FrameworkPropertyMetadata"></xref> is that specific WPF framework-level properties in the metadata such as <xref href="System.Windows.FrameworkPropertyMetadata.AffectsRender"></xref> are combined in a bitwise or operation.  
  
 The <xref href="System.Windows.FrameworkPropertyMetadata.Merge(System.Windows.PropertyMetadata,System.Windows.DependencyProperty)"></xref> behavior also implements the behavior when you override the property metadata on an existing dependency property by calling <xref href="System.Windows.DependencyProperty.OverrideMetadata(System.Type,System.Windows.PropertyMetadata)"></xref>., using override metadata that is <xref href="System.Windows.FrameworkPropertyMetadata"></xref>.</p>


