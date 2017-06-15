---
uid: System.Collections.DictionaryBase.OnSet(System.Object,System.Object,System.Object)
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed before setting the specified element in the underlying <xref href="System.Collections.Hashtable"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.DictionaryBase.OnSet(System.Object,System.Object,System.Object)"></xref> is invoked before the standard Set behavior, whereas <xref href="System.Collections.DictionaryBase.OnSetComplete(System.Object,System.Object,System.Object)"></xref> is invoked after the standard Set behavior.  
  
 For example, implementers can restrict which values can be overwritten by performing a check inside <xref href="System.Collections.DictionaryBase.OnSet(System.Object,System.Object,System.Object)"></xref>.</p>


