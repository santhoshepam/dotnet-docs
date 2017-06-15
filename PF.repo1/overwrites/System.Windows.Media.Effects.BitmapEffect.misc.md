---
uid: System.Windows.Media.Effects.BitmapEffect
additional_notes.overrides: *content
---

<p>
      <xref href="System.Windows.Media.Effects.BitmapEffect.CreateUnmanagedEffect"></xref> must be overridden to initialize an unmanaged effect in managed code.  
  
 <xref href="System.Windows.Media.Effects.BitmapEffect.UpdateUnmanagedPropertyState(System.Runtime.InteropServices.SafeHandle)"></xref> must be overridden when an unmanaged effect has properties that the user can modify. Use this method in conjunction with <xref href="System.Windows.Media.Effects.BitmapEffect.SetValue(System.Runtime.InteropServices.SafeHandle,System.String,System.Object)"></xref> to update your unmanaged properties.</p>


