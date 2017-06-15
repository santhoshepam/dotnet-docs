---
uid: System.Web.UI.WebControls.WebParts.GenericWebPart
additional_notes.overrides: *content
---

<p>There are few occasions where it is necessary to inherit from the <xref href="System.Web.UI.WebControls.WebParts.GenericWebPart"></xref> class. One such case would be if a developer wants to implement some custom action in the constructor when a <xref href="System.Web.UI.WebControls.WebParts.GenericWebPart"></xref> control is created. For example, you might want to store the child control somewhere other than the control collection within the <xref href="System.Web.UI.WebControls.WebParts.GenericWebPart"></xref> class. If you inherit from the <xref href="System.Web.UI.WebControls.WebParts.GenericWebPart"></xref> class, you also need to inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class and override its <xref href="System.Web.UI.WebControls.WebParts.WebPartManager.CreateWebPart(System.Web.UI.Control)"></xref> method to enable it to create your custom control.</p>


