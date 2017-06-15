---
uid: System.Drawing.Design.ToolboxService.CreateItemContainer(System.Drawing.Design.ToolboxItem,System.ComponentModel.Design.IDesignerHost)
additional_notes.overrides: *content
---

<p>A linked toolbox item is one whose existence is tied to the storage of a particular designer host. So, in a typical project system, a designer host is associated with a particular file. A toolbox item linked to a designer host would automatically be deleted from the toolbox when the designer host’s source file is deleted or removed from the project.  
  
 Linked toolbox items make possible scenarios such as disabling the [!INCLUDE[vstecasp](~/includes/vstecasp-md.md)] toolbox items when the Windows Forms designer is open.</p>


