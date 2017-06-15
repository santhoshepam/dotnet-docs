---
uid: System.Text.Encoding.GetEncoder
additional_notes.overrides: *content
---

<p>The default implementation returns a <xref href="System.Text.Encoder"></xref> that calls the <xref href="System.Text.Encoding.GetByteCount(System.Char[])"></xref> and <xref href="System.Text.Encoding.GetBytes(System.Char[])"></xref> methods of the current <xref href="System.Text.Encoding"></xref>. You must override this method to return a <xref href="System.Text.Encoder"></xref> that maintains its state between calls.</p>


