---
uid: System.Web.Hosting.VirtualPathProvider.CombineVirtualPaths(System.String,System.String)
additional_notes.overrides: *content
---

<p>If you override the default implementation of the <xref href="System.Web.Hosting.VirtualPathProvider.CombineVirtualPaths(System.String,System.String)"></xref> method, you are required to convert any special syntax with the <code>relativePath</code> parameter to a valid virtual path. You are responsible for syntax checking, path validation, and handling malformed input, as well as edge cases for well-formed input.  
  
 In most cases it will not be necessary to override the default <xref href="System.Web.Hosting.VirtualPathProvider.CombineVirtualPaths(System.String,System.String)"></xref> method. However, if you do need to modify the path, we recommend that you limit your <xref href="System.Web.Hosting.VirtualPathProvider.CombineVirtualPaths(System.String,System.String)"></xref> implementation to modifying tokens specific to your virtual path provider in the <code>relativeUrl</code> parameter, and that you then call the base implementation to perform normal ASP.NET path processing</p>


