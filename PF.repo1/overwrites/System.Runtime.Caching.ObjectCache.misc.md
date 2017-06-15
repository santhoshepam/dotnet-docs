---
uid: System.Runtime.Caching.ObjectCache
thread_safety: *content
---

This type is thread safe.


---
uid: System.Runtime.Caching.ObjectCache
additional_notes.overrides: *content
---

<p>Because the <xref href="System.Runtime.Caching.ObjectCache"></xref> type represents only common cache functions, there is no requirement for how an <xref href="System.Runtime.Caching.ObjectCache"></xref> instance must be instantiated and obtained. In addition, there is no requirement that concrete implementations of the <xref href="System.Runtime.Caching.ObjectCache"></xref> class must be singletons.  
  
 <block subset="none" type="note"><p><xref href="System.Runtime.Caching.MemoryCache"></xref> is not a singleton, but you should create only a few or potentially only one <xref href="System.Runtime.Caching.MemoryCache"></xref> instance and code that caches items should use those instances.  
  
</p></block>  
  
 When you inherit from the <xref href="System.Runtime.Caching.ObjectCache"></xref> class, you must override its methods.</p>


