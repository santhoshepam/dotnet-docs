---
uid: System.Windows.Interop.HwndHost.MeasureOverride(System.Windows.Size)
additional_notes.overrides: *content
---

<p>In [!INCLUDE[TLA#tla_win32](~/includes/tlasharptla-win32-md.md)], a window is expected to be the size requested by layout at the time the window is created. Derived classes should override this method only if they have additional information regarding required window size.  
  
 The specific implementation here is already an override of the <xref href="System.Windows.FrameworkElement"></xref> virtual member, which bases size constraints on the window handle and treats a zero value in one or more dimensions as a non-constraint. The <xref href="System.Windows.Forms.Integration.WindowsFormsHost"></xref> class also overrides a <xref href="System.Windows.Forms.Integration.WindowsFormsHost.MeasureOverride(System.Windows.Size)"></xref> implementation that will result in a clip of the form if it is too large.</p>


