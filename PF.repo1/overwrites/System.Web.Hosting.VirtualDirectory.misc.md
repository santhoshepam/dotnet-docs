---
uid: System.Web.Hosting.VirtualDirectory
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.Hosting.VirtualDirectory"></xref> class, you must override the <xref href="System.Web.Hosting.VirtualDirectory.Children"></xref>, <xref href="System.Web.Hosting.VirtualDirectory.Directories"></xref>, and <xref href="System.Web.Hosting.VirtualDirectory.Files"></xref> properties to return an object implementing the <xref href="System.Collections.IEnumerable"></xref> interface.  
  
 If your virtual-directory structure contains moderate to large numbers of virtual resources, you should take care to minimize the system resources consumed when enumerating the virtual directory by calling the <xref href="System.Web.Hosting.VirtualDirectory.Children"></xref>, <xref href="System.Web.Hosting.VirtualDirectory.Directories"></xref>, or <xref href="System.Web.Hosting.VirtualDirectory.Files"></xref> properties.</p>


