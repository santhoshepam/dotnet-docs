---
uid: System.Windows.ContentElement.Focusable
additional_notes.overrides: *content
---

<p>When you derive from <xref href="System.Windows.ContentElement"></xref>, consider whether you want your element to be focusable, because by default it will not be focusable. If you want your element to be focusable, override the metadata for this property in your derived class static constructor as follows:  
  
 [!code-csharp[CorePseudocode#UIElementShortOverride](~/samples/snippets/csharp/VS_Snippets_Wpf/CorePseudocode/CSharp/corepseudocode.cs#uielementshortoverride)]
 [!code-vb[CorePseudocode#UIElementShortOverride](~/samples/snippets/visualbasic/VS_Snippets_Wpf/CorePseudocode/visualbasic/corepseudocode.vb#uielementshortoverride)]  
  
 where <code>myElement</code> is the class name of the type that you are overriding the metadata value on.</p>


