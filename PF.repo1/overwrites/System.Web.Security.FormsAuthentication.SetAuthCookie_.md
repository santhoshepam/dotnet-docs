---
summary: Creates an authentication ticket for the supplied user name and adds it to the cookies collection of the response, or to the URL if you are using cookieless authentication.
remarks: The <xref:System.Web.Security.FormsAuthentication.SetAuthCookie%2A> method adds a forms-authentication ticket to either the cookies collection or the URL if <xref:System.Web.Security.FormsAuthentication.CookiesSupported%2A> is `false`. The forms-authentication ticket supplies forms-authentication information to the next request made by the browser. With forms authentication, you can use the <xref:System.Web.Security.FormsAuthentication.SetAuthCookie%2A> method when you want to authenticate a user but still retain control of the navigation with redirects.
uid: System.Web.Security.FormsAuthentication.SetAuthCookie*
---
