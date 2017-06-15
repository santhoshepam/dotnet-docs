---
uid: System.Windows.FrameworkElement.ArrangeOverride(System.Windows.Size)
additional_notes.overrides: *content
---

<p>Control authors who want to customize the arrange pass of layout processing should override this method. The implementation pattern should call <xref href="System.Windows.UIElement.Arrange(System.Windows.Rect)"></xref> on each visible child element, and pass the final desired size for each child element as the <code>finalRect</code> parameter. Parent elements should call <xref href="System.Windows.UIElement.Arrange(System.Windows.Rect)"></xref> on each child, otherwise the child elements will not be rendered.  
  
 Many derived classes offer implementations of this method. Prominent ones include: <xref href="System.Windows.Window.ArrangeOverride(System.Windows.Size)"></xref>, <xref href="System.Windows.Controls.Page.ArrangeOverride(System.Windows.Size)"></xref> and <xref href="System.Windows.Controls.Control.ArrangeOverride(System.Windows.Size)"></xref>.</p>


