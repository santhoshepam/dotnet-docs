---
uid: System.Web.Util.HttpEncoder
additional_notes.overrides: *content
---

<p>When you create a custom encoder class and override the base methods of the base class, the derived encoder might throw an exception from any of the overridden methods. However, in the following cases throwing such an exception could lead to unexpected behavior in ASP.NET:  
  
-   If ASP.NET is rendering an error page that is caused by an unhandled exception that was thrown from a custom encoder, ASP.NET does not attempt to encode its error output by calling into the custom encoder. This avoids recursive error conditions.  
  
-   When ASP.NET is sending HTTP headers to IIS, ASP.NET has no provision for unhandled exceptions. Therefore, the standard ASP.NET error page will be rendered (if configuration settings allows this page to be displayed).</p>


