---
uid: System.Collections.CollectionBase.OnValidate(System.Object)
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed when executing the standard behavior of the underlying <xref href="System.Collections.ArrayList"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.CollectionBase.OnValidate(System.Object)"></xref> can be used to impose restrictions on the type of objects that are accepted into the collection. The default implementation prevents `null` from being added to or removed from the underlying <xref href="System.Collections.ArrayList"></xref>.  
  
 <xref href="System.Collections.CollectionBase.OnValidate(System.Object)"></xref> is called prior to <xref href="System.Collections.CollectionBase.OnInsert(System.Int32,System.Object)"></xref>, <xref href="System.Collections.CollectionBase.OnRemove(System.Int32,System.Object)"></xref>, and <xref href="System.Collections.CollectionBase.OnSet(System.Int32,System.Object,System.Object)"></xref>.</p>


