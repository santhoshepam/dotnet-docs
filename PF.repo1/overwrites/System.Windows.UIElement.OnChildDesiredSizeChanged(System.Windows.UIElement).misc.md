---
uid: System.Windows.UIElement.OnChildDesiredSizeChanged(System.Windows.UIElement)
additional_notes.overrides: *content
---

<p>The <xref href="System.Windows.UIElement.OnChildDesiredSizeChanged(System.Windows.UIElement)"></xref> method has the default implementation of calling <xref href="System.Windows.UIElement.InvalidateMeasure"></xref> on itself. A typical implementation would be: do whatever optimization your own element supports, and then typically call base <xref href="System.Windows.UIElement.OnChildDesiredSizeChanged(System.Windows.UIElement)"></xref> from at least one of the code branches (the one that indicated "dirty" state per your own measure caching logic).  
  
 This method is only called in the layout processing if it was the child itself that originated the size changes. Otherwise, if the parent element initiates the <xref href="System.Windows.UIElement.Measure(System.Windows.Size)"></xref> pass, according to the layout system rules, the parent is recalculating layout already. The layout system processes layout in the order of child-to-parent, so no return to parent element sizing from the child element layout calls is necessary.</p>


