---
uid: System.Text.EncodingProvider.GetEncoding(System.String,System.Text.EncoderFallback,System.Text.DecoderFallback)
additional_notes.overrides: *content
---

<p>Because calls to this method use your implementation of the <xref href="System.Text.EncodingProvider.GetEncoding(System.String)"></xref> method, you do not have to override it. When user code attempts to retrieve an encoding by calling the <xref href="System.Text.EncodingProvider.GetEncoding(System.String,System.Text.EncoderFallback,System.Text.DecoderFallback)"></xref> method, the method passes the <code>codepage</code> identifier to every registered encoding provider until one returns a valid encoding. If none returns a valid encoding, the <xref href="System.Text.Encoding.GetEncoding(System.Int32)"></xref> method attempts to retrieve a cached encoding whose code page identifier is <code>codepage</code>. Because of this, if you do choose to override the <xref href="System.Text.EncodingProvider.GetEncoding(System.Int32,System.Text.EncoderFallback,System.Text.DecoderFallback)"></xref> method, your override should return `null` if <code>codepage</code> is not the code page identifier of an encoding that you support; it should never throw an exception.</p>


---
uid: System.Text.EncodingProvider.GetEncoding(System.String,System.Text.EncoderFallback,System.Text.DecoderFallback)
additional_notes.usage: *content
---

<p>This method is called by the <xref href="System.Text.Encoding.GetEncoding(System.String,System.Text.EncoderFallback,System.Text.DecoderFallback)"></xref> method. You should not call it directly from user code.</p>


