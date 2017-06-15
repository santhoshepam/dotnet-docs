---
uid: System.Windows.UIElement.MeasureCore(System.Windows.Size)
additional_notes.overrides: *content
---

<p>Implementations must be able to process a value provided for <code>availableSize</code> that is infinite. An infinite value indicates no requested constraints, and effectively defers measurement choice to the parent element, through recursive Measure calls.  
  
 Implementations can consider the value provided for <code>availableSize</code> to be a soft constraint. The child element might specify a larger size, even if other aspects of application code were able to determine the current actual size of the parent element. The large size request is a convention that indicates that the child element is querying whether your parent element can support content scrolling within a content display region.</p>


