---
uid: System.Windows.FrameworkElement.OnStyleChanged(System.Windows.Style,System.Windows.Style)
additional_notes.overrides: *content
---

<p>You should not typically have to override this method. Any change to a style that involves a measure or arrange change would already trigger another render cycle, assuming a typical implementation of <xref href="System.Windows.FrameworkElement.ArrangeOverride(System.Windows.Size)"></xref> / <xref href="System.Windows.FrameworkElement.MeasureOverride(System.Windows.Size)"></xref>, or the defaults. Overrides of <xref href="System.Windows.FrameworkElement.OnStyleChanged(System.Windows.Style,System.Windows.Style)"></xref> might be appropriate if your <xref href="System.Windows.FrameworkElement.ArrangeOverride(System.Windows.Size)"></xref> / <xref href="System.Windows.FrameworkElement.MeasureOverride(System.Windows.Size)"></xref> implementations were deliberately optimizing or supporting partial updates, but still wanted to apply changes to styles more directly. (The partial updates would be an attempt to avoid multiple incremental calls to <xref href="System.Windows.UIElement.Measure(System.Windows.Size)"></xref> and <xref href="System.Windows.UIElement.Arrange(System.Windows.Rect)"></xref> on any child elements).</p>


