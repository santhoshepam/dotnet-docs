---
uid: System.IO.BinaryReader.Dispose(System.Boolean)
additional_notes.overrides: *content
---

<p>
      <xref href="System.IO.BinaryReader.Dispose(System.Boolean)"></xref> can be called multiple times by other objects. When overriding this method, be careful not to reference objects that have been previously disposed of in an earlier call to `Dispose`. For more information about how to implement this method, see [Implementing a Dispose Method](~/docs/standard/garbage-collection/implementing-dispose.md).  
  
 For more information about <xref href="System.IDisposable.Dispose"></xref> and <xref href="System.Object.Finalize"></xref>, see [Cleaning Up Unmanaged Resources](~/docs/standard/garbage-collection/unmanaged.md).</p>


