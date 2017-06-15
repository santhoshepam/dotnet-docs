---
uid: System.Net.Sockets.TcpListener.Stop
additional_notes.usage: *content
---

<p>The <xref href="System.Net.Sockets.TcpListener.Stop"></xref> method also closes the underlying <xref href="System.Net.Sockets.Socket"></xref>, and creates a new <xref href="System.Net.Sockets.Socket"></xref> for the <xref href="System.Net.Sockets.TcpListener"></xref>. If you set any properties on the underlying <xref href="System.Net.Sockets.Socket"></xref> prior to calling the <xref href="System.Net.Sockets.TcpListener.Stop"></xref> method, those properties will not carry over to the new <xref href="System.Net.Sockets.Socket"></xref>.</p>


