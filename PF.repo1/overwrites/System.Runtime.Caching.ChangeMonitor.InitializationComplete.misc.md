---
uid: System.Runtime.Caching.ChangeMonitor.InitializationComplete
additional_notes.overrides: *content
---

<p>The constructor of a derived class must call the base <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method before the constructor returns. The constructor of a derived class can call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method only after <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> is called, because the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method throws an exception if initialization is not completed.</p>


