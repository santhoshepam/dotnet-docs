---
uid: System.Windows.IWeakEventListener.ReceiveWeakEvent(System.Type,System.Object,System.EventArgs)
additional_notes.overrides: *content
---

<p>This method is intended to receive all possible events where the receiver is in a listener list. Particularly if implementing for a class that is listening for more than one event, you must check the type of the incoming <code>managerType</code> parameter in order to know which event the call corresponds to. This is why each event that is to be part of the pattern must have a dedicated <xref href="System.Windows.WeakEventManager"></xref>. Also, the <code>e</code> parameter is typed as the general <xref href="System.EventArgs"></xref>. Therefore, in order get any specific properties out of the event data, your implementation will need to cast to the specific event data type.  
  
 Typically, after checking for the identity of the event based on the <xref href="System.Windows.WeakEventManager"></xref> type, your implementation should call a private class handler. Your class handler could conceivably be the very same class handler that is used to handle that event for listeners that are added through the conventional event pattern of adding via `+=` to the event on the sender. The following example section provides a rough implementation template.</p>


