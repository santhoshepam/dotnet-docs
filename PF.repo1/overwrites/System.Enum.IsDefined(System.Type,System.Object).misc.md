---
uid: System.Enum.IsDefined(System.Type,System.Object)
additional_notes.usage: *content
---

<p>If <code>enumType</code> is an enumeration that is defined by using the <xref href="System.FlagsAttribute"></xref> attribute, the method returns `false` if multiple bit fields in <code>value</code> are set but <code>value</code> does not correspond to a composite enumeration value, or if <code>value</code> is a string concatenation of the names of multiple bit flags. In the following example, a <code>Pets</code> enumeration is defined with the <xref href="System.FlagsAttribute"></xref> attribute. The <xref href="System.Enum.IsDefined(System.Type,System.Object)"></xref> method returns `false` when you pass it an enumeration value that has two bit fields (<code>Pets.Dog</code> and <code>Pets.Cat</code>) set, and when you pass it the string representation of that enumeration value ("Dog, Cat").  
  
 [!code-csharp[System.Enum.IsDefined#2](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.Enum.IsDefined/cs/isdefined2.cs#2)]
 [!code-vb[System.Enum.IsDefined#2](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.Enum.IsDefined/vb/isdefined2.vb#2)]  
  
 You can determine whether multiple bit fields are set by calling the <xref href="System.Enum.HasFlag(System.Enum)"></xref> method.</p>


