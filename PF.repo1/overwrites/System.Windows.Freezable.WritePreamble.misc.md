---
uid: System.Windows.Freezable.WritePreamble
additional_notes.overrides: *content
---

<p>Classes that derive from <xref href="System.Windows.Freezable"></xref> should call <xref href="System.Windows.Freezable.WritePreamble"></xref> before attempting to write to any members that are not dependency properties. If you call <xref href="System.Windows.Freezable.WritePreamble"></xref> in an [!INCLUDE[TLA#tla_api](~/includes/tlasharptla-api-md.md)], you can omit a call to <xref href="System.Windows.Freezable.ReadPreamble"></xref>.</p>


