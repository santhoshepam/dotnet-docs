---
uid: System.IO.Stream.Dispose(System.Boolean)
additional_notes.overrides: *content
---

<p>In derived classes, do not override the <xref href="System.IO.Stream.Close"></xref> method, instead, put all of the Stream cleanup logic in the <xref href="System.IO.Stream.Dispose(System.Boolean)"></xref> method.  
  
 <xref href="System.ComponentModel.Component.Dispose"></xref> can be called multiple times by other objects. When overriding <xref href="System.IO.Stream.Dispose(System.Boolean)"></xref>, be careful not to reference objects that have been previously disposed of in an earlier call to <xref href="System.ComponentModel.Component.Dispose"></xref>. For more information about how to implement <xref href="System.IO.Stream.Dispose(System.Boolean)"></xref>, see [Implementing a Dispose Method](~/docs/standard/garbage-collection/implementing-dispose.md).  
  
 For more information about <xref href="System.ComponentModel.Component.Dispose"></xref> and <xref href="System.Object.Finalize"></xref>, see [Cleaning Up Unmanaged Resources](~/docs/standard/garbage-collection/unmanaged.md).</p>


