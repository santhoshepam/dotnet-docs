---
uid: System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)
additional_notes.overrides: *content
---

<p>The derived <xref href="System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)"></xref> implementation should make no assumptions about the order or operations performed by the <xref href="System.IO.Packaging.PackagePart.GetStream*"></xref> method that calls it.</p>


---
uid: System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)
additional_notes.usage: *content
---

<p>The derived <xref href="System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)"></xref> method is called by the <xref href="System.IO.Packaging.PackagePart.GetStream*"></xref> methods to open and return the part data stream based on the physical format implemented in the derived class.  
  
 By default, the <xref href="System.IO.Packaging.ZipPackagePart"></xref> subclass implementation of the abstract <xref href="System.IO.Packaging.PackagePart"></xref> class is provided and used.  In the default operation, <xref href="System.IO.Packaging.PackagePart.GetStream*"></xref> internally calls <xref href="System.IO.Packaging.PackagePart.GetStreamCore(System.IO.FileMode,System.IO.FileAccess)"></xref> of the <xref href="System.IO.Packaging.ZipPackagePart"></xref> class to open and return the part data stream from a ZIP file.</p>


