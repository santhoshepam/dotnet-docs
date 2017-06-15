---
uid: System.Windows.Forms.IContainerControl
additional_notes.overrides: *content
---

<p>Implement this interface in classes that you want to parent a collection of controls. The members of this interface allow you to activate a child control, or determine which control is currently active. When implemented in a class, <xref href="System.Windows.Forms.IContainerControl.ActivateControl(System.Windows.Forms.Control)"></xref> takes a <xref href="System.Windows.Forms.Control"></xref> as a parameter and activates the specified control. The <xref href="System.Windows.Forms.IContainerControl.ActiveControl"></xref> property activates or retrieves the control that is active.  
  
 In most common scenarios, you do not need to directly implement this interface. For example, if you create a Windows Control Library project, Visual Studio generates an initial class for you. That class inherits from the <xref href="System.Windows.Forms.UserControl"></xref> class, and <xref href="System.Windows.Forms.UserControl"></xref> implements <xref href="System.Windows.Forms.IContainerControl"></xref> for you.</p>


