---
uid: System.Security.HostSecurityManager
additional_notes.overrides: *content
---

<p>Some members of a <xref href="System.Security.HostSecurityManager"></xref> are called whenever an assembly is loaded, either implicitly or explicitly. The <xref href="System.Security.HostSecurityManager.ProvideAssemblyEvidence(System.Reflection.Assembly,System.Security.Policy.Evidence)"></xref> and <xref href="System.Security.HostSecurityManager.ProvideAppDomainEvidence(System.Security.Policy.Evidence)"></xref> methods must not load any assemblies, because doing so will result in the members of the <xref href="System.Security.HostSecurityManager"></xref> being recursively called. To avoid circular references, you should create new instances of classes that can cause assemblies to be loaded, either implicitly or explicitly, in the constructor of a class that derives from <xref href="System.Security.HostSecurityManager"></xref>.</p>


