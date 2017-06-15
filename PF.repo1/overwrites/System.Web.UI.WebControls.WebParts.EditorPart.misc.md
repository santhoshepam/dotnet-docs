---
uid: System.Web.UI.WebControls.WebParts.EditorPart
additional_notes.overrides: *content
---

<p>To create a custom <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> control, you must override two important methods. The <xref href="System.Web.UI.WebControls.WebParts.EditorPart.ApplyChanges"></xref> method applies changes made in the editor control to the <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control being edited. The <xref href="System.Web.UI.WebControls.WebParts.EditorPart.SyncChanges"></xref> method gets the current values of the <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control being edited, so that the editor control can edit them. Using these two critical methods, you get and set values between your custom <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> control and the <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control it is editing.  
  
 If you derive from the <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> class to create custom editor controls, you can add your custom controls to an <xref href="System.Web.UI.WebControls.WebParts.EditorZoneBase"></xref> zone by implementing the <xref href="System.Web.UI.WebControls.WebParts.IWebEditable"></xref> interface in a <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control, a user control, or a server control. For more details and a code example, see the <xref href="System.Web.UI.WebControls.WebParts.IWebEditable"></xref> class overview. Also, the code example in the Example section demonstrates how to implement <xref href="System.Web.UI.WebControls.WebParts.IWebEditable"></xref> in a custom <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control.</p>


