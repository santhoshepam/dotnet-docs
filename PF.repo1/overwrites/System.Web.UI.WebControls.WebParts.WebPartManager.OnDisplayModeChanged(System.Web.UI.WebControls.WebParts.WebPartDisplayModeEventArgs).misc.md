---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.OnDisplayModeChanged(System.Web.UI.WebControls.WebParts.WebPartDisplayModeEventArgs)
additional_notes.overrides: *content
---

<p>You can override the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.OnDisplayModeChanged(System.Web.UI.WebControls.WebParts.WebPartDisplayModeEventArgs)"></xref> method. For example, after a change of display mode, you might want to change something in the appearance of the user interface (UI), depending on which display mode is contained in the <xref href="System.Web.UI.WebControls.WebParts.WebPartDisplayModeEventArgs.OldDisplayMode"></xref> property. Or you might want to hide certain content, or display a certain control.  
  
 When you override the method, you should normally call the base method as the last step of the overridden method, so that your custom code runs first, and the event is raised last, indicating that the mode change is complete.</p>


