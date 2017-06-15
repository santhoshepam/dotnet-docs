---
uid: System.Resources.ResourceManager.#ctor(System.String,System.Reflection.Assembly,System.Type)
additional_notes.usage: *content
---

<p>This constructor lets you specify a <xref href="System.Resources.ResourceSet"></xref> implementation. If you do not want a specific <xref href="System.Resources.ResourceSet"></xref> implementation but would like to use a custom resource file format, you should derive from the <xref href="System.Resources.ResourceSet"></xref> class, override the <xref href="System.Resources.ResourceSet.GetDefaultReader"></xref> and <xref href="System.Resources.ResourceSet.GetDefaultWriter"></xref> methods, and pass that type to this constructor.</p>


