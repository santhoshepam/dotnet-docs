---
uid: System.Web.Hosting.VirtualFile.Open
additional_notes.overrides: *content
---

<p>In derived classes the <xref href="System.Web.Hosting.VirtualFile.Open"></xref> method must return a seekable stream. If the method returns a stream that does not support seeking, a <xref href="System.NotSupportedException"></xref> is thrown when the stream is passed to the <xref href="System.Web.HttpResponse"></xref> object to write out the data. The exception occurs because the response tries to read the <xref href="System.IO.Stream.Length"></xref> property, and on a stream that is not seekable, attempting to access the property causes an exception. For more information, see the <xref href="System.IO.Stream.CanSeek"></xref> property.</p>


