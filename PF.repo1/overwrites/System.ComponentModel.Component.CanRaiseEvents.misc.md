---
uid: System.ComponentModel.Component.CanRaiseEvents
additional_notes.overrides: *content
---

<p>If you override this method in a deriving class and change it to return `false`, the <xref href="System.ComponentModel.EventHandlerList"></xref> collection returned by the <xref href="System.ComponentModel.Component.Events"></xref> property returns `null` for an event. Events can still be added and removed from the collection, but the collection's <xref href="System.ComponentModel.EventHandlerList.Item(System.Object)"></xref> property will always return `null`.</p>


