---
uid: System.Windows.FrameworkElement.OnPropertyChanged(System.Windows.DependencyPropertyChangedEventArgs)
additional_notes.overrides: *content
---

<p>Always call the base implementation, as the first operation in your implementation. Failure to do this will significantly disable the entire [!INCLUDE[TLA2#tla_winclient](~/includes/tla2sharptla-winclient-md.md)] property system, which causes incorrect values to be reported. The specific <xref href="System.Windows.FrameworkElement"></xref> implementation is also responsible for maintaining proper state for a variety of properties that affect the visible user interface. These include invalidating the visual tree based on changes to style at appropriate times.</p>


