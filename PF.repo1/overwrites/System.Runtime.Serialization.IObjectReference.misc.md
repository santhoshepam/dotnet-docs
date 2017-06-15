---
uid: System.Runtime.Serialization.IObjectReference
additional_notes.overrides: *content
---

<p>Implement this interface on objects that are references to a different object, which cannot be resolved until the current object is completely restored. During the fixup stage, any object implementing <xref href="System.Runtime.Serialization.IObjectReference"></xref> is queried for its real object and that object is inserted into the graph. Fixup refers to the process of finalizing references not already completed during the object deserialization process.</p>


