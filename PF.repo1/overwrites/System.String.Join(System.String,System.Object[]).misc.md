---
uid: System.String.Join(System.String,System.Object[])
additional_notes.usage: *content
---

<p>If the first element of <code>values</code> is `null`, the <xref href="System.String.Join(System.String,System.Object[])"></xref> method does not concatenate the elements in <code>values</code> but instead returns <xref href="System.String.Empty"></xref>. A number of workarounds for this issue are available. The easiest is to assign a value of <xref href="System.String.Empty"></xref> to the first element of the array, as the following example shows.  
  
 [!code-csharp[System.String.Join#6](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.string.join/cs/joinfix1.cs#6)]
 [!code-vb[System.String.Join#6](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.string.join/vb/joinfix1.vb#6)]</p>


