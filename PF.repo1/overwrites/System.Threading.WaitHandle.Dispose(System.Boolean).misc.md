---
uid: System.Threading.WaitHandle.Dispose(System.Boolean)
additional_notes.overrides: *content
---

<p>You should override the <xref href="System.Threading.WaitHandle.Dispose(System.Boolean)"></xref> method to release resources allocated in derived classes.  
  
 The <xref href="System.Threading.WaitHandle.Close"></xref> or <xref href="System.Threading.WaitHandle.Dispose"></xref> method can be called multiple times by other objects. When overriding this method, be careful not to reference objects that have been previously disposed in an earlier call to `Dispose` or `Close`.</p>


