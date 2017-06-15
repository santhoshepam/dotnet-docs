---
uid: System.Array.Sort(System.Array,System.Collections.IComparer)
additional_notes.usage: *content
---

<p>The .NET Framework 4 and earlier versions used only the Quicksort algorithm. Quicksort identifies invalid comparers in some situations in which the sorting operation throws an <xref href="System.IndexOutOfRangeException"></xref> exception, and throws an <xref href="System.ArgumentException"></xref> exception to the caller. Starting with the [!INCLUDE[net_v45](~/includes/net-v45-md.md)], it is possible that sorting operations that previously threw <xref href="System.ArgumentException"></xref> will not throw an exception, because the insertion sort and heapsort algorithms do not detect an invalid comparer. For the most part, this applies to arrays with fewer than 16 elements.</p>


