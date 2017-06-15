---
uid: System.IdentityModel.Services.CookieHandler.DeleteCore(System.String,System.String,System.String,System.Web.HttpContext)
additional_notes.overrides: *content
---

<p>You must override this method. The implementation is entirely up to the developer. In the typical case, implementations replace the specified cookie in the <xref href="System.Web.HttpResponse.Cookies"></xref> collection, with a cookie that has `null` data and an expiration time that is set earlier than the current time; however, this is not a requirement.</p>


