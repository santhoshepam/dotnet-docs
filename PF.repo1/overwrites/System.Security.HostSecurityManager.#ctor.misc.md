---
uid: System.Security.HostSecurityManager.#ctor
additional_notes.overrides: *content
---

<p>Create instances of classes that can cause assemblies to be loaded, either explicitly or implicitly, in this constructor.  The get accessor for the <xref href="System.Security.HostSecurityManager.DomainPolicy"></xref> property and the <xref href="System.Security.HostSecurityManager.ProvideAssemblyEvidence(System.Reflection.Assembly,System.Security.Policy.Evidence)"></xref> and <xref href="System.Security.HostSecurityManager.ProvideAppDomainEvidence(System.Security.Policy.Evidence)"></xref> methods are called whenever an assembly is loaded, and their subsequent loading of assemblies will cause circular references.</p>


