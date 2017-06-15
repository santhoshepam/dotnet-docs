---
uid: System.Resources.ResourceManager.#ctor(System.String,System.Reflection.Assembly)
additional_notes.overrides: *content
---

<p>This constructor uses the system-provided <xref href="System.Resources.ResourceSet"></xref> implementation. To use a custom resource file format, you should derive from the <xref href="System.Resources.ResourceSet"></xref> class, override the <xref href="System.Resources.ResourceSet.GetDefaultReader"></xref> and <xref href="System.Resources.ResourceSet.GetDefaultWriter"></xref> methods, and pass that type to the <xref href="System.Resources.ResourceManager.#ctor(System.String,System.Reflection.Assembly,System.Type)"></xref> constructor. Using a custom <xref href="System.Resources.ResourceSet"></xref> can be useful for controlling resource caching policy or supporting your own resource file format, but is generally not necessary.</p>


