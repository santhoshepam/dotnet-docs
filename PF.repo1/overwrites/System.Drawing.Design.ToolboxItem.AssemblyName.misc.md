---
uid: System.Drawing.Design.ToolboxItem.AssemblyName
additional_notes.overrides: *content
---

<p>If your derived toolbox item class creates multiple components that are located in different assemblies, you must ensure that references to these assemblies exist in your project. It is advisable to add these references from an overload of the <xref href="System.Drawing.Design.ToolboxItem.CreateComponentsCore(System.ComponentModel.Design.IDesignerHost)"></xref> method. Even if your <xref href="System.Drawing.Design.ToolboxItem.CreateComponentsCore(System.ComponentModel.Design.IDesignerHost)"></xref> method does not depend on the value of the <xref href="System.Drawing.Design.ToolboxItem.AssemblyName"></xref> property, you should ensure that this property is set to the assembly that one of the components to create belongs to, because it is displayed in the **Customize Toolbox** dialog box in [!INCLUDE[vsprvs](~/includes/vsprvs-md.md)].</p>


