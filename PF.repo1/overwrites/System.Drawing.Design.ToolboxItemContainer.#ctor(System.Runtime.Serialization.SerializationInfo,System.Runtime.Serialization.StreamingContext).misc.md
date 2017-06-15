---
uid: System.Drawing.Design.ToolboxItemContainer.#ctor(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)
additional_notes.overrides: *content
---

<p>
      <xref href="System.Drawing.Design.ToolboxItemContainer"></xref> objects can be serialized. Generally, it is not necessary to override the serialization mechanism for a <xref href="System.Drawing.Design.ToolboxItemContainer"></xref>. <xref href="System.Drawing.Design.ToolboxItemContainer"></xref> objects implement serialization by saving the <xref href="System.Windows.Forms.IDataObject"></xref> returned from the <xref href="System.Drawing.Design.ToolboxItemContainer.ToolboxData"></xref> property. When you override <xref href="System.Drawing.Design.ToolboxItemContainer.ToolboxData"></xref> and provide your own custom data, this data is included with the default <xref href="System.Runtime.Serialization.ISerializable"></xref> implementation. Override the default serialization implementation only if you intend to store private details about this <xref href="System.Drawing.Design.ToolboxItemContainer"></xref> that should not be exposed through the public data object.</p>


