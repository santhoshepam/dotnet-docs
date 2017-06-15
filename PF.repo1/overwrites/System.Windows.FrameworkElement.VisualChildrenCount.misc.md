---
uid: System.Windows.FrameworkElement.VisualChildrenCount
additional_notes.overrides: *content
---

<p>If your class supports more than one visual child in a child element collection, override this property to return the count of elements in that collection. You must do this even if the collection object itself returns a count. Element layout logic at the WPF framework level presumes that all elements will return a valid count through their <xref href="System.Windows.FrameworkElement.VisualChildrenCount"></xref> property.</p>


