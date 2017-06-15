---
uid: System.Text.Encoding.GetDecoder
additional_notes.overrides: *content
---

<p>The default implementation returns a <xref href="System.Text.Decoder"></xref> that calls the <xref href="System.Text.Encoding.GetCharCount(System.Byte[])"></xref> and <xref href="System.Text.Encoding.GetChars(System.Byte[])"></xref> methods of the current <xref href="System.Text.Encoding"></xref>. You must override this method to return a <xref href="System.Text.Decoder"></xref> that maintains its state between calls.</p>


