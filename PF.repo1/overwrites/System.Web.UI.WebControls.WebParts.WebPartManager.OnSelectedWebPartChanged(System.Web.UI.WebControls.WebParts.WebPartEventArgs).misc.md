---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.OnSelectedWebPartChanged(System.Web.UI.WebControls.WebParts.WebPartEventArgs)
additional_notes.overrides: *content
---

<p>There are several options related to the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.SelectedWebPartChanged"></xref> event, to allow developers to customize the rendering that occurs after the selected control has changed. In declarative code, within the `<asp:webpartmanager>` element you could set the `OnSelectedWebPartChanged` attribute, and assign to it the name of a custom method. In the custom method, you could modify the rendering of the selected controls when the event occurs. Another option is to inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class and override the method. A third option is to customize the rendering at the zone level; for example, you can inherit from the <xref href="System.Web.UI.WebControls.WebParts.EditorZoneBase"></xref> class, and override its <xref href="System.Web.UI.WebControls.WebParts.EditorZoneBase.OnSelectedWebPartChanged(System.Object,System.Web.UI.WebControls.WebParts.WebPartEventArgs)"></xref> method, to customize the rendering of controls selected and cleared during the editing process.</p>


