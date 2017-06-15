---
uid: System.Windows.WeakEventManager.Purge(System.Object,System.Object,System.Boolean)
additional_notes.overrides: *content
---

<p>If the underlying type for the <xref href="System.Windows.WeakEventManager.Item(System.Object)"></xref> is something other than <xref href="System.Windows.WeakEventManager.ListenerList"></xref>, or contains data beyond a <xref href="System.Windows.WeakEventManager.ListenerList"></xref>, you must override the <xref href="System.Windows.WeakEventManager.Purge(System.Object,System.Object,System.Boolean)"></xref> method. The override should provide purge behavior for the alternate type items list. Generally, the override should provide behavior without calling the base implementation. If a specific <xref href="System.Windows.WeakEventManager.ListenerList"></xref> still needs clearing, call <xref href="System.Windows.WeakEventManager.ListenerList.Purge"></xref>.</p>


