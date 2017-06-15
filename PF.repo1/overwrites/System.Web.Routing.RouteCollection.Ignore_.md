---
summary: Defines a URL pattern that should not be checked for matches against routes.
remarks: "This method creates a route that is mapped to the <xref:System.Web.Routing.StopRoutingHandler> route handler. After you call this method, requests that match the specified URL pattern will not be processed as route requests.  \n  \n ASP.NET routing automatically ignores requests when the URL matches a physical file, such as an image file. In some cases you might also want routing to ignore requests when there is no physical file. For example, the requests that ASP.NET automatically makes for .axd files should not be treated as route requests even though there is no physical file that corresponds to the .axd file-name extension."
uid: System.Web.Routing.RouteCollection.Ignore*
---
