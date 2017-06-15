---
uid: System.Windows.FrameworkElement.GetVisualChild(System.Int32)
additional_notes.overrides: *content
---

<p>This implementation is only valid for elements that do not maintain any more descriptive collection of visual child elements. Any element that does have such a collection must override this method and map the index to an equivalent index in the child element collection that is supported by that element. An index in the range from zero to <xref href="System.Windows.FrameworkElement.VisualChildrenCount"></xref> (minus one) should return a valid element; any other index should throw an out-of-range exception. An example of an element type that does support a child collection and overrides <xref href="System.Windows.FrameworkElement.GetVisualChild(System.Int32)"></xref> to return more than one possible child is <xref href="System.Windows.Controls.Panel"></xref>.  
  
 The default implementation in <xref href="System.Windows.FrameworkElement"></xref> presumes only one visual child. Any value passed for <code>index</code> other than zero causes an exception to be thrown. Several common elements, such as decorators, adorners, or elements with specialized rendering, override the <xref href="System.Windows.FrameworkElement"></xref> implementation (of the implementation from intermediate base classes). Some implementations still enforce one visual child whereas others allow a collection.</p>


