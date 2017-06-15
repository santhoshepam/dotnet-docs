---
uid: System.Globalization.CultureInfo.#ctor(System.String)
additional_notes.usage: *content
---

<p>The [!INCLUDE[net_v35_long](~/includes/net-v35-long-md.md)] and earlier versions throw an <xref href="System.ArgumentException"></xref> if <code>name</code> is not a valid culture name. Starting with the [!INCLUDE[net_v40_long](~/includes/net-v40-long-md.md)], this constructor throws a <xref href="System.Globalization.CultureNotFoundException"></xref>. Starting with apps that run under the [!INCLUDE[net_v40_long](~/includes/net-v40-long-md.md)] or later on Windows 7 or later, the method attempts to retrieve a <xref href="System.Globalization.CultureInfo"></xref> object whose identifier is <code>name</code> from the operating system; if the operating system does not support that culture, and if <code>name</code> is not the name of a supplementary or replacement culture, the method throws a <xref href="System.Globalization.CultureNotFoundException"></xref> exception.</p>


