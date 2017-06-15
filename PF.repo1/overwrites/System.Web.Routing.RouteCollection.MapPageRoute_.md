---
summary: Provides a way to define routes for Web Forms applications.
remarks: This method is provided for coding convenience. It is equivalent to calling the <xref:System.Web.Routing.RouteCollection.Add%2A> method and passing a <xref:System.Web.Routing.Route> object that is created by using the <xref:System.Web.Routing.PageRouteHandler> class.
example:
- "The following example shows how to define routes for a Web Forms application by using this method. The example shows a method named `RegisterRoutes` that is called from `Application_Start` in the Global.asax file. The method uses each overload of <xref:System.Web.Routing.RouteCollection.MapPageRoute%2A> to add a route to the application. For more information about how to define routes for Web Forms applications, see [How to: Define Routes for Web Forms Applications](http://msdn.microsoft.com/library/200fe812-d0a6-4531-b9b4-cfc4ee83a678).  \n  \n [!code-csharp[System.Web.Routing.RouteCollection.MapPageRoute#122](~/samples/snippets/csharp/VS_Snippets_WebNet/system.web.routing.routecollection.mappageroute/cs/global.asax#122)]\n [!code-vb[System.Web.Routing.RouteCollection.MapPageRoute#122](~/samples/snippets/visualbasic/VS_Snippets_WebNet/system.web.routing.routecollection.mappageroute/vb/global.asax#122)]"
uid: System.Web.Routing.RouteCollection.MapPageRoute*
---
