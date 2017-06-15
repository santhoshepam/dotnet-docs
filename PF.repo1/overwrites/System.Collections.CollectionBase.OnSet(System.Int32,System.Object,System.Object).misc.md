---
uid: System.Collections.CollectionBase.OnSet(System.Int32,System.Object,System.Object)
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed before setting the specified element in the underlying <xref href="System.Collections.ArrayList"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.CollectionBase.OnSet(System.Int32,System.Object,System.Object)"></xref> is invoked before the standard Set behavior, whereas <xref href="System.Collections.CollectionBase.OnSetComplete(System.Int32,System.Object,System.Object)"></xref> is invoked after the standard Set behavior.  
  
 For example, implementers can restrict which values can be overwritten by performing a check inside <xref href="System.Collections.CollectionBase.OnSet(System.Int32,System.Object,System.Object)"></xref>.  
  
 <xref href="System.Collections.CollectionBase.OnValidate(System.Object)"></xref> is called prior to this method.</p>


