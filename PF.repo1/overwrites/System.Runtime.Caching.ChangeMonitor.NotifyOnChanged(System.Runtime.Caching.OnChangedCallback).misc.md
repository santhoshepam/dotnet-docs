---
uid: System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)
additional_notes.overrides: *content
---

<p>1.  You must call the <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> method to be notified of any dependency changes. If a dependency change has already occurred, the <xref href="System.Runtime.Caching.OnChangedCallback"></xref> instance will be called when <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> is called. Otherwise, the <xref href="System.Runtime.Caching.OnChangedCallback"></xref> instance will be called one time, either when the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method is called or when the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method is called, whichever occurs first. The <xref href="System.Runtime.Caching.OnChangedCallback"></xref> instance provided by the cache implementation should remove the cache entry and if it is requested by the cache caller, raise the necessary change or update event back to the original cache caller.  
  
2.  The object cache implementation must remove the cache entry that is associated with a dependency change.</p>


