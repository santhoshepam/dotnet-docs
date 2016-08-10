---
uid: System.Text.Encoding.UTF8
remarks: |
 This property returns a @System.Text.UTF8Encoding object that encodes Unicode (UTF-16-encoded) characters into a sequence of one to four bytes per character, and that decodes a UTF-8-encoded byte array to Unicode (UTF-16-encoded) characters. For information about the character encodings supported by the .NET Framework and a discussion of which Unicode encoding to use, see [Character Encoding in the .NET Framework](https://msdn.microsoft.com/en-us/library/ms404377(v=vs.110).aspx).
 The @System.Text.UTF8Encoding object that is returned by this property might not have the appropriate behavior for your app.
 - It returns a @System.Text.UTF8Encoding object that provides a Unicode byte order mark (BOM). To instantiate a UTF8 encoding that doesn't provide a BOM, call any overload of the @System.Text.UTF8Encoding.%23ctor constructor.
 - It returns a @System.Text.UTF8Encoding object that uses replacement fallback to replace each string that it can't encode and each byte that it can't decode with a question mark ("?") character. Instead, you can call the @System.Text.UTF8Encoding.#ctor(System.Boolean,System.Boolean) constructor to instantiate a @System.Text.UTF8Encoding object whose fallback is either an @System.Text.EncoderFallbackException or a @System.Text.DecoderFallbackException.
---