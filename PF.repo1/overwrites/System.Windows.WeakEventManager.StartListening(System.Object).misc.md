---
uid: System.Windows.WeakEventManager.StartListening(System.Object)
additional_notes.overrides: *content
---

<p>
      <xref href="System.Windows.WeakEventManager.StartListening(System.Object)"></xref> overrides should add a handler to the provided <code>source</code>. The handler is declared by the manager itself. The class handler should not be public, and it should only be called in response to the event being managed. The class handler should call the <xref href="System.Windows.WeakEventManager.DeliverEvent(System.Object,System.EventArgs)"></xref> method or the <xref href="System.Windows.WeakEventManager.DeliverEventToList(System.Object,System.EventArgs,System.Windows.WeakEventManager.ListenerList)"></xref> method appropriately.</p>


