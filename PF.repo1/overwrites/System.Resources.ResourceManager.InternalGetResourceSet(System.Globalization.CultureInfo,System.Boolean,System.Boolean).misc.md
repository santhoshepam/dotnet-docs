---
uid: System.Resources.ResourceManager.InternalGetResourceSet(System.Globalization.CultureInfo,System.Boolean,System.Boolean)
additional_notes.overrides: *content
---

<p>This method completes all the work necessary to find a resource set, and can be recursive and reentrant. In other words, this method might load an assembly and trigger an <xref href="System.AppDomain.AssemblyLoad"></xref> event, which then calls back into a <xref href="System.Resources.ResourceManager"></xref> object that has not been completely initialized. To avoid taking extra locks, this method is not thread safe. The <xref href="System.Resources.ResourceManager.GetResourceSet(System.Globalization.CultureInfo,System.Boolean,System.Boolean)"></xref>, <xref href="System.Resources.ResourceManager.GetString(System.String)"></xref>, and <xref href="System.Resources.ResourceManager.GetObject(System.String)"></xref> methods do all the necessary synchronization.</p>


