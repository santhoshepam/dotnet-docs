---
uid: System.Text.StringBuilder.Append(System.Char[])
additional_notes.usage: *content
---

<p>In the[!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)] and the [!INCLUDE[net_v45](~/includes/net-v45-md.md)], when you instantiate the <xref href="System.Text.StringBuilder"></xref> object by calling the <xref href="System.Text.StringBuilder.#ctor(System.Int32,System.Int32)"></xref> constructor, both the length and the capacity of the <xref href="System.Text.StringBuilder"></xref> instance can grow beyond the value of its <xref href="System.Text.StringBuilder.MaxCapacity"></xref> property. This can occur particularly when you call the <xref href="System.Text.StringBuilder.Append(System.String)"></xref> and <xref href="System.Text.StringBuilder.AppendFormat(System.String,System.Object)"></xref> methods to append small strings.</p>


