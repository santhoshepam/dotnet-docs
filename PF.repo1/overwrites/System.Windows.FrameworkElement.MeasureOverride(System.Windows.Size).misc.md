---
uid: System.Windows.FrameworkElement.MeasureOverride(System.Windows.Size)
additional_notes.overrides: *content
---

<p>The following non-compiling code shows this implementation pattern.  <code>VisualChildren</code> represents an enumerable collection property of children that your own element should define. The property can be named anything. <code>VisualChildren</code> is a placeholder name for purposes of this example, <code>VisualChildren</code> is not an [!INCLUDE[TLA#tla_api](~/includes/tlasharptla-api-md.md)] as provided by [!INCLUDE[TLA2#tla_winclient](~/includes/tla2sharptla-winclient-md.md)] or a part of a naming pattern..  
  
 [!code-csharp[CorePseudocode#FEMeasureOverride](~/samples/snippets/csharp/VS_Snippets_Wpf/CorePseudocode/CSharp/corepseudocode.cs#femeasureoverride)]
 [!code-vb[CorePseudocode#FEMeasureOverride](~/samples/snippets/visualbasic/VS_Snippets_Wpf/CorePseudocode/visualbasic/corepseudocode.vb#femeasureoverride)]</p>


