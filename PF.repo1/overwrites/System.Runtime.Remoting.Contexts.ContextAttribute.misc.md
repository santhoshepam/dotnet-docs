---
uid: System.Runtime.Remoting.Contexts.ContextAttribute
additional_notes.overrides: *content
---

<p>The <xref href="System.Runtime.Remoting.Contexts.ContextAttribute.Name"></xref> property must not be overridden in any user derived class. The current <xref href="System.Runtime.Remoting.Contexts.ContextAttribute.Equals(System.Object)"></xref> and <xref href="System.Runtime.Remoting.Contexts.ContextAttribute.GetHashCode"></xref> methods depend on the default functionality. To provide advanced behavior for a class extending the <xref href="System.Runtime.Remoting.Contexts.ContextAttribute"></xref> class and override the <xref href="System.Runtime.Remoting.Contexts.ContextAttribute.Name"></xref> property, you also have to override the default implementation of the <xref href="System.Runtime.Remoting.Contexts.ContextAttribute.Equals(System.Object)"></xref> and <xref href="System.Runtime.Remoting.Contexts.ContextAttribute.GetHashCode"></xref> methods.</p>


