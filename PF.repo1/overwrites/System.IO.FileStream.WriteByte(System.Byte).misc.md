---
uid: System.IO.FileStream.WriteByte(System.Byte)
additional_notes.overrides: *content
---

<p>The default implementation on `Stream` creates a new single-byte array and then calls <xref href="System.IO.Stream.Write(System.Byte[],System.Int32,System.Int32)"></xref>. While this is formally correct, it is inefficient. Any stream with an internal buffer should override this method and provide a much more efficient version that reads the buffer directly, avoiding the extra array allocation on every call.  
  
 For a list of common file and directory operations, see [Common I/O Tasks](~/docs/standard/io/common-i-o-tasks.md).</p>


