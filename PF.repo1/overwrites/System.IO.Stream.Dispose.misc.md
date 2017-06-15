---
uid: System.IO.Stream.Dispose
additional_notes.overrides: *content
---

<p>Place all cleanup logic for your stream object in <xref href="System.IO.Stream.Dispose(System.Boolean)"></xref>. Do not override <xref href="System.IO.Stream.Close"></xref>.  
  
 Note that because of backward compatibility requirements, this method's implementation differs from the recommended guidance for the Dispose pattern.  This method calls <xref href="System.IO.Stream.Close"></xref>, which then calls <xref href="System.IO.Stream.Dispose(System.Boolean)"></xref>.</p>


