---
uid: System.IO.Packaging.PackagePart.GetStream(System.IO.FileMode,System.IO.FileAccess)
additional_notes.usage: *content
---

<p>
      <xref href="System.IO.Packaging.PackagePart.GetStream(System.IO.FileMode,System.IO.FileAccess)"></xref> internally calls the derived <xref href="System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)"></xref> method to actually open and return the part data stream based on the physical format implemented in the derived class.  
  
 By default, the <xref href="System.IO.Packaging.ZipPackagePart"></xref> subclass implementation of the abstract <xref href="System.IO.Packaging.PackagePart"></xref> class is provided and used.  In the default operation, <xref href="System.IO.Packaging.PackagePart.GetStream(System.IO.FileMode,System.IO.FileAccess)"></xref> internally calls <xref href="System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)"></xref> of the <xref href="System.IO.Packaging.ZipPackagePart"></xref> class to open and return the part data stream from a ZIP file.</p>


