---
uid: System.Windows.PropertyMetadata.Merge(System.Windows.PropertyMetadata,System.Windows.DependencyProperty)
additional_notes.overrides: *content
---

<p>Class implementations that derive from <xref href="System.Windows.PropertyMetadata"></xref> should override this method to account for any metadata properties they have added in their implementations. For instance, your implementation might have added a new flagwise enumeration value, and the <xref href="System.Windows.PropertyMetadata.Merge(System.Windows.PropertyMetadata,System.Windows.DependencyProperty)"></xref> implementation should then be able to combine those flags correctly.  
  
 Always call the base implementation prior to your implementation code, because the base implementation takes care of merging all the properties already defined on the <xref href="System.Windows.PropertyMetadata"></xref> type.  
  
 The exact behavior of the merge is up to you. You could choose to have values combined, revert to base value if the derived metadata were left at the default, or many other behaviors based on the types of properties you have added to your particular metadata class, and their meanings.</p>


