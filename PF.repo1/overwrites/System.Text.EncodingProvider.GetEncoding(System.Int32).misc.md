---
uid: System.Text.EncodingProvider.GetEncoding(System.Int32)
additional_notes.overrides: *content
---

<p>You override the <xref href="System.Text.EncodingProvider.GetEncoding(System.Int32)"></xref> method to return the encoding or encodings supported by your <xref href="System.Text.EncodingProvider"></xref> subclass. When user code attempts to retrieve an encoding by calling the <xref href="System.Text.Encoding.GetEncoding(System.Int32)"></xref> method, the method passes the <code>codepage</code> identifier to every registered encoding provider until one returns a valid encoding. If none returns a valid encoding, the <xref href="System.Text.Encoding.GetEncoding(System.Int32)"></xref> method attempts to retrieve a cached encoding whose code page identifier is <code>codepage</code>. Because of this, if <code>codepage</code> is not the code page identifier of an encoding that you support, the method should return `null`; it should never throw an exception.</p>


---
uid: System.Text.EncodingProvider.GetEncoding(System.Int32)
additional_notes.usage: *content
---

<p>This method is called by the <xref href="System.Text.Encoding.GetEncoding(System.Int32)"></xref> method. You should not call it directly from user code.</p>


