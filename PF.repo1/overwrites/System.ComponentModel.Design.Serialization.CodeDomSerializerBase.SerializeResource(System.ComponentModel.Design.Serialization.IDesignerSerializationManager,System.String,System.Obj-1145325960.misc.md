---
uid: System.ComponentModel.Design.Serialization.CodeDomSerializerBase.SerializeResource(System.ComponentModel.Design.Serialization.IDesignerSerializationManager,System.String,System.Object)
additional_notes.usage: *content
---

<p>
      `ResourceCulture` is a read-write property that is accessed through the serialization manager’s <xref href="System.ComponentModel.Design.Serialization.IDesignerSerializationManager.Properties"></xref> collection. The <xref href="System.ComponentModel.Design.Serialization.CodeDomSerializerBase.SerializeResource(System.ComponentModel.Design.Serialization.IDesignerSerializationManager,System.String,System.Object)"></xref> method never changes the value of this property; it merely reads it to identify the culture to which it will write. The property is set during deserialization as resources are parsed and loaded.</p>


