---
uid: System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)
additional_notes.overrides: *content
---

<p>A change monitor must implement the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)"></xref> overload to release all managed and unmanaged resources when the value of <code>disposing</code> is `true`. The <xref href="System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)"></xref> method overload that has a <code>disposing</code> value of `true` is called only one time, namely, when the instance is disposed for the first time. A change monitor must not call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)"></xref> overload directly. A derived change monitor can call the public parameter-less <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method on the base <xref href="System.Runtime.Caching.ChangeMonitor"></xref> class.  
  
 Alternatively, a change monitor can implement a finalizer method. In that case, the finalizer can invoke the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)"></xref> method and pass it a <code>disposing</code> value of `false`. However, this is usually unnecessary. Monitoring for dependency changes is typically performed by a service that maintains a reference to the change-monitor instance. The reference prevents the instance from being garbage collected, and therefore makes a finalizer method unnecessary. To avoid memory leaks, when a dependency changes, the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method disposes the change-monitor instance (unless initialization has not finished).</p>


