---
uid: System.Collections.CollectionBase.OnInsert(System.Int32,System.Object)
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed before inserting the element into the underlying <xref href="System.Collections.ArrayList"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.CollectionBase.OnInsert(System.Int32,System.Object)"></xref> is invoked before the standard Insert behavior, whereas <xref href="System.Collections.CollectionBase.OnInsertComplete(System.Int32,System.Object)"></xref> is invoked after the standard Insert behavior.  
  
 For example, implementers can restrict which types of objects can be inserted into the <xref href="System.Collections.ArrayList"></xref>.  
  
 <xref href="System.Collections.CollectionBase.OnValidate(System.Object)"></xref> is called prior to this method.</p>


