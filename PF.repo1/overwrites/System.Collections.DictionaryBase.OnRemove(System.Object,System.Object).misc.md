---
uid: System.Collections.DictionaryBase.OnRemove(System.Object,System.Object)
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed before removing the element from the underlying <xref href="System.Collections.Hashtable"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.DictionaryBase.OnRemove(System.Object,System.Object)"></xref> is invoked before the standard Remove behavior, whereas <xref href="System.Collections.DictionaryBase.OnRemoveComplete(System.Object,System.Object)"></xref> is invoked after the standard Remove behavior.  
  
 For example, implementers can prevent removal of elements by always throwing an exception in <xref href="System.Collections.DictionaryBase.OnRemove(System.Object,System.Object)"></xref>.</p>


