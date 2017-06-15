---
uid: System.IdentityModel.Selectors.SecurityTokenProvider.BeginCancelTokenCore(System.TimeSpan,System.IdentityModel.Tokens.SecurityToken,System.AsyncCallback,System.Object)
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.IdentityModel.Selectors.SecurityTokenProvider"></xref> class you are not required to override the asynchronous methods, as the <xref href="System.IdentityModel.Selectors.SecurityTokenProvider"></xref> base class provides asynchronous support based upon the synchronous methods. Therefore, you are not required to override the <xref href="System.IdentityModel.Selectors.SecurityTokenProvider.BeginCancelTokenCore(System.TimeSpan,System.IdentityModel.Tokens.SecurityToken,System.AsyncCallback,System.Object)"></xref> method, unless you need to provide your own asynchronous implementation.  
  
 The <xref href="System.IdentityModel.Selectors.SecurityTokenProvider.BeginCancelTokenCore(System.TimeSpan,System.IdentityModel.Tokens.SecurityToken,System.AsyncCallback,System.Object)"></xref> method is called by the <xref href="System.IdentityModel.Selectors.SecurityTokenProvider.BeginCancelToken(System.TimeSpan,System.IdentityModel.Tokens.SecurityToken,System.AsyncCallback,System.Object)"></xref> method.  
  
 The asynchronous methods, which have a prefix of Begin and End, do not need to be overridden in derived classes. The <xref href="System.IdentityModel.Selectors.SecurityTokenProvider"></xref> base class provides an asynchronous implementation that is based on the synchronous methods.</p>


