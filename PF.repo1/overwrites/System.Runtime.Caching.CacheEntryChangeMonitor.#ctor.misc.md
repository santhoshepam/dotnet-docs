---
uid: System.Runtime.Caching.CacheEntryChangeMonitor.#ctor
additional_notes.overrides: *content
---

<p>The constructor of a derived class must set the <xref href="System.Runtime.Caching.ChangeMonitor.UniqueId"></xref> property, begin monitoring, and call <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> before the constructor returns. If a dependency changes before initialization is complete (for example, if a dependent cache key is not found in the cache), the constructor must call the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method. The constructor can call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method only after <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> is called, because <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> throws an exception if initialization is not completed.</p>


