---
uid: System.Web.StaticSiteMapProvider.BuildSiteMap
additional_notes.overrides: *content
---

<p>When overriding the <xref href="System.Web.StaticSiteMapProvider.BuildSiteMap"></xref> method in a derived class, be sure to normalize the URLs of <xref href="System.Web.SiteMapNode"></xref> objects that you add to your site map provider, so that the <xref href="System.Web.StaticSiteMapProvider.FindSiteMapNode(System.String)"></xref> method can retrieve a site map node regardless of whether the URL for the site map node is supplied as an absolute virtual path or application relative path. Site map provider implementers using the <xref href="System.Web.StaticSiteMapProvider.AddNode*"></xref> method should normalize any URLs before storing <xref href="System.Web.SiteMapNode"></xref> objects in the internal hash tables on behalf of the site map provider.  
  
 Security trimming behavior is included in the <xref href="System.Web.SiteMapProvider"></xref> and <xref href="System.Web.StaticSiteMapProvider"></xref> class implementations. However, for security trimming to function in derived classes, you must set the <xref href="System.Web.SiteMapNode.Roles"></xref> property of any <xref href="System.Web.SiteMapNode"></xref> objects that you create while building a site map provider when you override the <xref href="System.Web.StaticSiteMapProvider.BuildSiteMap"></xref> method.</p>


