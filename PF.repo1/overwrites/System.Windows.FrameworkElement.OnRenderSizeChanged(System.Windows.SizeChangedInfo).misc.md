---
uid: System.Windows.FrameworkElement.OnRenderSizeChanged(System.Windows.SizeChangedInfo)
additional_notes.overrides: *content
---

<p>Do not override this method for typical layout scenarios. The layout system operates in a deliberately asynchronous way to assure that all possible layout arrange and measure cases are accounted for. The layout system override methods <xref href="System.Windows.FrameworkElement.MeasureOverride(System.Windows.Size)"></xref> and <xref href="System.Windows.FrameworkElement.ArrangeOverride(System.Windows.Size)"></xref> are usually sufficient for any required layout customization. <xref href="System.Windows.FrameworkElement.OnRenderSizeChanged(System.Windows.SizeChangedInfo)"></xref> is exposed as a virtual. You can override <xref href="System.Windows.FrameworkElement.OnRenderSizeChanged(System.Windows.SizeChangedInfo)"></xref> to correct for exceptional cases where a run-time behavioral change related to input events combined with control recomposition in response might give inaccurate layout information.  
  
 You may still override this method in derived classes (it is protected but not sealed). Always call the base implementation to preserve the behavior mentioned above, unless you have very specific reasons for disabling default WPF framework-level rendering behavior. Failing to raise the <xref href="System.Windows.FrameworkElement.SizeChanged"></xref> event will cause non-standard layout behavior if using the standard WPF framework-level layout system implementation.</p>


