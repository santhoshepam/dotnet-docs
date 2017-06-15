---
uid: System.ICloneable
additional_notes.overrides: *content
---

<p>The <xref href="System.ICloneable"></xref> interface simply requires that your implementation of the <xref href="System.ICloneable.Clone"></xref> method return a copy of the current object instance. It does not specify whether the cloning operation performs a deep copy, a shallow copy, or something in between. Nor does it require all property values of the original instance to be copied to the new instance. For example, the <xref href="System.Globalization.NumberFormatInfo.Clone"></xref> method performs a shallow copy of all properties except the <xref href="System.Globalization.NumberFormatInfo.IsReadOnly"></xref> property; it always sets this property value to `false` in the cloned object. Because callers of <xref href="System.ICloneable.Clone"></xref> cannot depend on the method performing a predictable cloning operation, we recommend that <xref href="System.ICloneable"></xref> not be implemented in public APIs.</p>


