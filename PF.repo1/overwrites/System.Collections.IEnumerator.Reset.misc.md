---
uid: System.Collections.IEnumerator.Reset
additional_notes.overrides: *content
---

<p>All calls to <xref href="System.Collections.IEnumerator.Reset"></xref> must result in the same state for the enumerator. The preferred implementation is to move the enumerator to the beginning of the collection, before the first element. This invalidates the enumerator if the collection has been modified since the enumerator was created, which is consistent with <xref href="System.Collections.IEnumerator.MoveNext"></xref> and <xref href="System.Collections.IEnumerator.Current"></xref>.</p>


