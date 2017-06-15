---
uid: System.Runtime.Caching.ChangeMonitor
thread_safety: *content
---

This type is thread safe.


---
uid: System.Runtime.Caching.ChangeMonitor
additional_notes.overrides: *content
---

<p>If you create a custom cache implementation or a derived change monitor type, you must follow certain guidelines. The following list summarizes these guidelines. For more information, see the documentation for individual methods or properties.  
  
-   The constructor of a derived class must set the <xref href="System.Runtime.Caching.ChangeMonitor.UniqueId"></xref> property, begin monitoring, and call <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method before the method returns. If a constructor encounters an error during constructions and must have to dispose of resources, the constructor can only call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> overload after the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method is called because the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> overload will throw an <xref href="System.InvalidOperationException"></xref> exception if initialization is not completed.  
  
-   If changes occur in the data that is being monitored before initialization is complete, the constructor must call the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method before calling the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method.  
  
-   After a derived <xref href="System.Runtime.Caching.ChangeMonitor"></xref> type is instantiated, you must insert the monitor into a custom <xref href="System.Runtime.Caching.ObjectCache"></xref> implementation. Or if you are finished using the change monitor, call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> method.  
  
-   After a <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instance is inserted into a <xref href="System.Runtime.Caching.ObjectCache"></xref> implementation, the <xref href="System.Runtime.Caching.ObjectCache"></xref> instance require that the change monitor is disposed. Even if the insertion is invalid and causes an exception, the <xref href="System.Runtime.Caching.ObjectCache"></xref> implementation must call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> overload.  
  
-   After a derived change monitor is inserted into a cache, the <xref href="System.Runtime.Caching.ObjectCache"></xref> implementation must call <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref>, by passing a <xref href="System.Runtime.Caching.OnChangedCallback"></xref> object. The <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> method can be called only one time. If a dependency change has already occurred, the <xref href="System.Runtime.Caching.OnChangedCallback"></xref> instance will be called immediately when <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> is called. Otherwise, the <xref href="System.Runtime.Caching.OnChangedCallback"></xref> instance will be called only one time. This one time call occurs either when the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method is called because the <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instance detected a change, or when the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method is called on the <xref href="System.Runtime.Caching.ChangeMonitor"></xref>, whichever occurs first.  
  
-   The <xref href="System.Runtime.Caching.OnChangedCallback"></xref> instance that is provided by an <xref href="System.Runtime.Caching.ObjectCache"></xref> implementation should remove the associated cache entry and specify a reason by using the <xref href="System.Web.Caching.CacheItemRemovedReason.DependencyChanged"></xref> enumeration.  
  
-   A <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instance can call the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method either before a cache implementation has called <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> method or after. If the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method is called before <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> is called, the base <xref href="System.Runtime.Caching.ChangeMonitor"></xref> implementation will notify the cache that this has occurred and will trigger the callback to be passed to <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> immediately when <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> is invoked. Any state data that is passed to the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method is saved by the change monitor and subsequently passed to the <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> method when the <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> method is invoked.  
  
-   A change monitor must implement the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)"></xref> method. For more information, see the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose(System.Boolean)"></xref> method documentation.  
  
-   The <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method overload must be called to dispose of the <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instance. The rules for calling Dispose are as follows:  
  
    -   Before an item is inserted into the cache, it is the responsibility of caller to dispose of a <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instance.  
  
    -   Once cache item and the <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instances that are associated with it are passed to a cache, the cache implementer must make sure that that the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> method is called, even if the insert fails.  
  
    -   After an item and its associated <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instances are passed to a cache, the caller must not dispose the dependency because when the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> method is called, the call is treated as if the dependency has changed. As a result, the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method is automatically invoked.  
  
-   Taking these rules into consideration, the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> method must be called in one of the following ways:  
  
    -   Users must call the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> method overload if they decide not to insert the derived change-monitor instance into a cache.  
  
    -   If the implementation tries to insert the change-monitor instance into an object cache but the insertion fails, the cache implementation is responsible for calling the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose"></xref> overload. When the insertion attempt causes an exception, the cache implementation must dispose of any associated dependencies.  
  
    -   If the cache entry is removed, the cache implementation must also dispose of the dependency.  
  
    -   The internal implementation of the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method automatically calls the <xref href="System.Runtime.Caching.ChangeMonitor.Dispose*"></xref> method after it calls a callback that is registered through <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref>.  
  
 <block subset="none" type="note"><p>  
 This automatic call to the dispose method during the event firing only occurs if the initialization of the <xref href="System.Runtime.Caching.ChangeMonitor"></xref> instance was previously completed.  
  
</p></block>  
  
 When a derived change monitor's constructor calls the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method, if the state of the change monitor has already changed (that is, the state that is monitored already changed when the constructor was still active) then the <xref href="System.Runtime.Caching.ChangeMonitor.InitializationComplete"></xref> method will automatically dispose of the change monitor.  
  
-   The <xref href="System.Runtime.Caching.ChangeMonitor.HasChanged"></xref> property is set to `true` after the <xref href="System.Runtime.Caching.ChangeMonitor.OnChanged(System.Object)"></xref> method is called by the derived change-monitor instance, regardless of whether a <xref href="System.Runtime.Caching.OnChangedCallback"></xref> object has been set by a call to the <xref href="System.Runtime.Caching.ChangeMonitor.NotifyOnChanged(System.Runtime.Caching.OnChangedCallback)"></xref> method or not.</p>


