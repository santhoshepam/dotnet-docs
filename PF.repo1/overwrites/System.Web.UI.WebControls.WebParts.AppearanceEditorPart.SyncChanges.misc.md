---
uid: System.Web.UI.WebControls.WebParts.AppearanceEditorPart.SyncChanges
additional_notes.overrides: *content
---

<p>The Web Parts control set calls the <xref href="System.Web.UI.WebControls.WebParts.AppearanceEditorPart.SyncChanges"></xref> method within the inherited <xref href="System.Web.UI.Control.OnPreRender(System.EventArgs)"></xref> method, so that if any changes occurred after the user last viewed the control prior to editing (for example, a shared administrative user made changes to the control that would affect all users), those changes would be evident during the editing process.  
  
 If you create a custom control, you can follow the same approach, and call the <xref href="System.Web.UI.WebControls.WebParts.AppearanceEditorPart.SyncChanges"></xref> method from the inherited <xref href="System.Web.UI.Control.OnPreRender(System.EventArgs)"></xref> method to ensure that any intervening changes are synchronized, but it is not necessary to do this.</p>


