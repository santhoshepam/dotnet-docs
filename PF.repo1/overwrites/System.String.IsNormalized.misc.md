---
uid: System.String.IsNormalized
additional_notes.usage: *content
---

<p>The <xref href="System.String.IsNormalized*"></xref> method returns `false` as soon as it encounters the first non-normalized character in a string. Therefore, if a string contains non-normalized characters followed by invalid Unicode characters, the <xref href="System.String.Normalize*"></xref> method will throw an <xref href="System.ArgumentException"></xref> although <xref href="System.String.IsNormalized*"></xref> returns `false`.</p>


