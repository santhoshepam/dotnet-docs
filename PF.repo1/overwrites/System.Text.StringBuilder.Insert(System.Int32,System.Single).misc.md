---
uid: System.Text.StringBuilder.Insert(System.Int32,System.Single)
additional_notes.usage: *content
---

<p>In the [!INCLUDE[net_v35SP1_long](~/includes/net-v35sp1-long-md.md)] and earlier versions, calls to this method threw an <xref href="System.ArgumentOutOfRangeException"></xref> if inserting <code>value</code> would cause the object's total length to exceed <xref href="System.Text.StringBuilder.MaxCapacity"></xref>. Starting with the [!INCLUDE[net_v40_long](~/includes/net-v40-long-md.md)], the method throws an <xref href="System.OutOfMemoryException"></xref>.</p>


