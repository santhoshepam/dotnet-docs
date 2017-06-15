---
uid: System.Drawing.Design.ToolboxItemContainer.GetObjectData(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)
additional_notes.overrides: *content
---

<p>Generally, it is not necessary to override the serialization mechanism for a <xref href="System.Drawing.Design.ToolboxItemContainer"></xref> class. Instead, override the <xref href="System.Drawing.Design.ToolboxItemContainer.ToolboxData"></xref> property and add your own data to the data object. The <xref href="System.Drawing.Design.ToolboxItemContainer.GetObjectData(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)"></xref> method internally uses the <xref href="System.Drawing.Design.ToolboxItemContainer.ToolboxData"></xref> property to create the serialization info. Override <xref href="System.Drawing.Design.ToolboxItemContainer.GetObjectData(System.Runtime.Serialization.SerializationInfo,System.Runtime.Serialization.StreamingContext)"></xref> only if you want to save private information about the <xref href="System.Drawing.Design.ToolboxItemContainer"></xref> that should not be saved as part of the public data object.</p>


