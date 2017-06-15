---
uid: System.Resources.ResourceSet.ReadResources
additional_notes.overrides: *content
---

<p>Derived classes of <xref href="System.Resources.ResourceSet"></xref> should explicitly call <xref href="System.Resources.ResourceSet.ReadResources"></xref> to load all the resources from the <xref href="System.Resources.IResourceReader"></xref> into <xref href="System.Resources.ResourceSet.Table"></xref>, generally either in the constructor or lazily on the first call to either <xref href="System.Resources.ResourceSet.GetString(System.String)"></xref> or <xref href="System.Resources.ResourceSet.GetObject(System.String)"></xref>. However, if your resource set and IResourceReader already have information about each other and have a more efficient way to load just a few select resources, this step can be skipped. To minimize working set, write your resource set in such a way that it queries your IResourceReader for only the resource values requested by your application.</p>


