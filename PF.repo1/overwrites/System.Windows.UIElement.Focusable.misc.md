---
uid: System.Windows.UIElement.Focusable
additional_notes.overrides: *content
---

<p>When deriving from <xref href="System.Windows.UIElement"></xref> directly (as opposed to from <xref href="System.Windows.Controls.Control"></xref>), consider whether you wish your element to be focusable, because by default the element will not be focusable. If you wish your element to be focusable, override the metadata for this property within your type's static constructor as follows:  
  
 [!code-csharp[CorePseudocode#UIElementShortOverride](~/samples/snippets/csharp/VS_Snippets_Wpf/CorePseudocode/CSharp/corepseudocode.cs#uielementshortoverride)]
 [!code-vb[CorePseudocode#UIElementShortOverride](~/samples/snippets/visualbasic/VS_Snippets_Wpf/CorePseudocode/visualbasic/corepseudocode.vb#uielementshortoverride)]  
  
 where <code>myElement</code> should be the class name of the type that you are overriding the metadata value on.</p>


