---
uid: System.Web.SiteMapProvider.GetChildNodes(System.Web.SiteMapNode)
additional_notes.overrides: *content
---

<p>When overriding the <xref href="System.Web.SiteMapProvider.GetChildNodes(System.Web.SiteMapNode)"></xref> method in a derived class, be sure to perform security trimming on the child nodes and ensure that the returned collection is read-only. The collection contains only the immediate children of the specified <code>node</code>.</p>


