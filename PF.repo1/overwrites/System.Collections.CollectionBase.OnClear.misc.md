---
uid: System.Collections.CollectionBase.OnClear
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed before deleting all the elements from the underlying <xref href="System.Collections.ArrayList"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.CollectionBase.OnClear"></xref> is invoked before the standard Clear behavior, whereas <xref href="System.Collections.CollectionBase.OnClearComplete"></xref> is invoked after the standard Clear behavior.  
  
 For example, implementers can exempt certain elements from deletion by a global Clear.</p>


