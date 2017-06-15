---
uid: System.Windows.Controls.DataGridRow.OnPropertyChanged(System.Windows.DependencyPropertyChangedEventArgs)
additional_notes.overrides: *content
---

<p>Always call the base implementation as the first operation in your implementation. Failure to do this will significantly disable the entire [!INCLUDE[TLA2#tla_winclient](~/includes/tla2sharptla-winclient-md.md)] property system, which causes incorrect values to be reported. The specific <xref href="System.Windows.Controls.DataGridRow"></xref> implementation is also responsible for maintaining the correct state for the <xref href="System.Windows.Controls.DataGridRow.AlternationIndex"></xref> property, which affects the visible user interface and invalidates the visual tree based on property value changes at appropriate times.</p>


