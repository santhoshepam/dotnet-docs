---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.OnDisplayModeChanging(System.Web.UI.WebControls.WebParts.WebPartDisplayModeCancelEventArgs)
additional_notes.overrides: *content
---

<p>You can override the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.OnDisplayModeChanging(System.Web.UI.WebControls.WebParts.WebPartDisplayModeCancelEventArgs)"></xref> method. For example, as a display mode is changing, you might want to check what the new display mode will be (by using the <xref href="System.Web.UI.WebControls.WebParts.WebPartDisplayModeCancelEventArgs.NewDisplayMode"></xref> property) and change something in the user interface (UI) based on what the new display mode will be. If you had a custom display mode, you might want to make certain controls visible if the custom mode is going to be the new display mode.  
  
 When you override this method, you should normally call the base method as the first step of the overridden method, so that the event is raised to indicate a display mode is starting to change. Then, your custom code can make changes in the user interface (UI) before the new display mode is actually displayed.</p>


