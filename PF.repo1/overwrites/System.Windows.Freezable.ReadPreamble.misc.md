---
uid: System.Windows.Freezable.ReadPreamble
additional_notes.overrides: *content
---

<p>Classes that derive from <xref href="System.Windows.Freezable"></xref> should call the <xref href="System.Windows.Freezable.ReadPreamble"></xref> method before they attempt to access any members that are not dependency properties. The <xref href="System.Windows.Freezable.WritePreamble"></xref> method should be called before any such members are written to.  
  
 This method effectively does nothing more than call <xref href="System.Windows.Threading.DispatcherObject.VerifyAccess"></xref>.</p>


