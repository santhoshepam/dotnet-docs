---
uid: System.Web.Hosting.VirtualPathProvider
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.Web.Hosting.VirtualPathProvider"></xref>, you must override the following members:  
  
-   <xref href="System.Web.Hosting.VirtualPathProvider.FileExists(System.String)"></xref>  
  
-   <xref href="System.Web.Hosting.VirtualPathProvider.GetFile(System.String)"></xref>  
  
 If your custom <xref href="System.Web.Hosting.VirtualPathProvider"></xref> class supports directories in the virtual file system, you must override the following members.  
  
-   <xref href="System.Web.Hosting.VirtualPathProvider.DirectoryExists(System.String)"></xref>  
  
-   <xref href="System.Web.Hosting.VirtualPathProvider.GetDirectory(System.String)"></xref><block subset="none" type="note"><p>  
 If your virtual file system will contain themes for the Web site (by creating a virtual <code>App_Themes</code> directory), your custom <xref href="System.Web.Hosting.VirtualPathProvider"></xref> class must support directories.  
  
</p></block>  
  
 A custom <xref href="System.Web.Hosting.VirtualPathProvider"></xref> class works with classes derived from the <xref href="System.Web.Hosting.VirtualFile"></xref> and <xref href="System.Web.Hosting.VirtualDirectory"></xref> classes. You should implement derived classes from these types to provide file and directory information from your virtual file system. For an example of a custom <xref href="System.Web.Hosting.VirtualFile"></xref> implementation, see the Example section of the <xref href="System.Web.Hosting.VirtualFile"></xref> class overview topic. For an example of a custom <xref href="System.Web.Hosting.VirtualDirectory"></xref> implementation, see the Example section of the <xref href="System.Web.Hosting.VirtualDirectory"></xref> class overview topic.</p>


