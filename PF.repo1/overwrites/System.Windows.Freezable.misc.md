---
uid: System.Windows.Freezable
thread_safety: *content
---

Any public `static` members of this type are thread safe. Any instance members are not guaranteed to be thread safe.  
  
 When the <xref href="System.Windows.Freezable.IsFrozen"></xref> property is `false`, a <xref href="System.Windows.Freezable"></xref> object can be accessed only from the thread on which it was created. Attempting to access it from another thread throws an <xref href="System.InvalidOperationException"></xref>. The <xref href="System.Windows.Threading.Dispatcher.Invoke*"></xref> and <xref href="System.Windows.Threading.Dispatcher.BeginInvoke*"></xref> methods provide support for marshalling to the correct thread.  
  
 When their <xref href="System.Windows.Freezable.IsFrozen"></xref> property is `true`, <xref href="System.Windows.Freezable"></xref> objects are free-threaded.  For more information, see [Freezable Objects Overview](~/docs/framework/wpf/advanced/freezable-objects-overview.md).


