---
summary: Initializes a new instance of the <xref href="System.Windows.Interop.HwndSourceParameters"></xref> class. Do not use the default constructor for <xref href="System.Windows.Interop.HwndSourceParameters"></xref>; see Remarks.
remarks: >-
  > [!IMPORTANT]

  >  Do not construct instances of this structure using the default (parameterless) constructor. An <xref:System.Windows.Interop.HwndSourceParameters> instance that is created by the default constructor results in <xref:System.Windows.Interop.HwndSourceParameters> that cannot be assigned a <xref:System.Windows.Interop.HwndSourceParameters.WindowName%2A> (even though the <xref:System.Windows.Interop.HwndSourceParameters.WindowName%2A> property appears to be settable). If such an instance is applied as the parameters for an <xref:System.Windows.Interop.HwndSource> constructor, the resulting <xref:System.Windows.Interop.HwndSource> cannot display a window.
uid: System.Windows.Interop.HwndSourceParameters.#ctor*
---
