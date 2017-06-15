---
uid: System.Windows.FrameworkElement.OnVisualParentChanged(System.Windows.DependencyObject)
additional_notes.overrides: *content
---

<p>The default implementation of this virtual method queries for the new parent, raises various initialization events, and sets internal flags about initialization state of the <xref href="System.Windows.FrameworkElement"></xref> as appropriate. Finally, it calls the successive base implementations as declared by <xref href="System.Windows.UIElement"></xref>, which in turn calls its base in <xref href="System.Windows.Media.Visual"></xref>. Always call the base implementation to preserve this behavior, otherwise the element tree behavior for this element when declared as a child of another element may not be as expected.  
  
 A few existing [!INCLUDE[TLA#tla_winclient](~/includes/tlasharptla-winclient-md.md)] classes override this method, for example: <xref href="System.Windows.Window.OnVisualParentChanged(System.Windows.DependencyObject)"></xref>, <xref href="System.Windows.Controls.ListBoxItem.OnVisualParentChanged(System.Windows.DependencyObject)"></xref>. The most common scenario is to enforce that the new parent must be a particular type. This might involve throwing an exception if the new parent failed some manner of type test. A specialized version of this scenario exists in implementations for list items and menu items, which do not make any sense outside a parent visual that owns an appropriate collection to store them in. Note that these cases do not necessarily raise exceptions, because there might be designer scenarios that rely on reparenting elements that are momentarily without their "regular" parents.  
  
 This method is also overridden in certain elements that are typically the root element, such as  <xref href="System.Windows.Window"></xref>. Another case is elements that are the apparent root element in markup but which autogenerate a greater infrastructure in a compiled logical tree (such as <xref href="System.Windows.Controls.Page"></xref>). The <xref href="System.Windows.Window"></xref> and <xref href="System.Windows.Controls.Page"></xref> implementations deliberately seal the method.</p>


