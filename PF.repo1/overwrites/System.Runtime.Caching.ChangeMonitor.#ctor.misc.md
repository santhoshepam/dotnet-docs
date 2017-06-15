---
uid: System.Runtime.Caching.ChangeMonitor.#ctor
additional_notes.overrides: *content
---

<p>The constructor of a derived class must set the <xref href="System.Runtime.Caching.ChangeMonitor.UniqueId"></xref> property, begin monitoring, and call the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> class before it returns. If a dependency changes before initialization is complete (for example, if a dependent cache key is not found in the cache), the constructor must call the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method before it calls the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method. In this case, constructor can call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method only after the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method is called, because the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method throws an exception if initialization is not completed.</p>


