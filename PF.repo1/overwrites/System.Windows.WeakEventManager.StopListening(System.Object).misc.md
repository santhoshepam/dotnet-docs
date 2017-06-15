---
uid: System.Windows.WeakEventManager.StopListening(System.Object)
additional_notes.overrides: *content
---

<p>
      <xref href="System.Windows.WeakEventManager.StopListening(System.Object)"></xref> implementations should remove the class handler as added by the <xref href="System.Windows.WeakEventManager.StartListening(System.Object)"></xref> method. Removing a listener should not clear the listener list. Instead, it should only disconnect the class handler (perhaps temporarily). Other methods are available for clearing the entire list, such as the <xref href="System.Windows.WeakEventManager.Purge(System.Object,System.Object,System.Boolean)"></xref> method with the <code>purgeAll</code> parameter set to `true`.</p>


