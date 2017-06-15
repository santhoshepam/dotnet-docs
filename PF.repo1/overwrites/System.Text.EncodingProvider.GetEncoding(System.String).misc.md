---
uid: System.Text.EncodingProvider.GetEncoding(System.String)
additional_notes.overrides: *content
---

<p>You override the <xref href="System.Text.EncodingProvider.GetEncoding(System.String)"></xref> method to return the encoding or encodings supported by your <xref href="System.Text.EncodingProvider"></xref> subclass. When user code attempts to retrieve an encoding by calling the <xref href="System.Text.Encoding.GetEncoding(System.String)"></xref> method, the method passes the <code>name</code> argument to every registered encoding provider until one returns a valid encoding. If none returns a valid encoding, the <xref href="System.Text.Encoding.GetEncoding(System.String)"></xref> method attempts to retrieve a cached encoding whose name is <code>name</code>. Because of this, if <code>name</code> is not the name of an encoding that you support, the method should return `null`. The only case in which the method should throw an exception is if <code>name</code> is `null`.</p>


---
uid: System.Text.EncodingProvider.GetEncoding(System.String)
additional_notes.usage: *content
---

<p>This method is called by the <xref href="System.Text.Encoding.GetEncoding(System.String)"></xref> method. You should not call it directly from user code.</p>


