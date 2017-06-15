---
uid: System.Windows.Threading.DispatcherObject
thread_safety: *content
---

Any public `static` members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 This object can be accessed only from the thread on which it was created. Attempts to access it from other threads will throw an <xref href="System.InvalidOperationException"></xref>. <xref href="System.Windows.Threading.Dispatcher.Invoke(System.Windows.Threading.DispatcherPriority,System.Delegate)"></xref> or <xref href="System.Windows.Threading.Dispatcher.BeginInvoke(System.Windows.Threading.DispatcherPriority,System.Delegate)"></xref> provide support for marshalling work to the correct thread.


