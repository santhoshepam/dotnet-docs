---
uid: System.Collections.DictionaryBase.OnGet(System.Object,System.Object)
additional_notes.overrides: *content
---

<p>This method allows implementers to define processes that must be performed when executing the standard Get behavior of the underlying <xref href="System.Collections.Hashtable"></xref>. By defining this method, implementers can add functionality to inherited methods without having to override all other methods.  
  
 <xref href="System.Collections.DictionaryBase.OnGet(System.Object,System.Object)"></xref> can be used to specify processes to perform before returning the value retrieved from the underlying <xref href="System.Collections.Hashtable"></xref>. For example, implementers can cast the value into another type before returning it.</p>


