---
uid: System.Web.StaticSiteMapProvider.FindSiteMapNode(System.String)
additional_notes.overrides: *content
---

<p>When overriding the <xref href="System.Web.StaticSiteMapProvider.FindSiteMapNode(System.String)"></xref> method in a derived class, be sure to normalize the URLs of the <xref href="System.Web.SiteMapNode"></xref> objects that you add to your site map provider, so that the <xref href="System.Web.StaticSiteMapProvider.FindSiteMapNode(System.String)"></xref> method can retrieve a site map node regardless of whether URL for the site map node is supplied as an absolute virtual path or an application relative path.  
  
 Security trimming behavior is included in the <xref href="System.Web.SiteMapProvider"></xref> and <xref href="System.Web.StaticSiteMapProvider"></xref> class implementations. However, for security trimming to function in derived classes, you must set the <xref href="System.Web.SiteMapNode.Roles"></xref> property of any <xref href="System.Web.SiteMapNode"></xref> objects that you create while building a site map provider when you override the <xref href="System.Web.StaticSiteMapProvider.BuildSiteMap"></xref> method.</p>


