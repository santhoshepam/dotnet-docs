---
uid: System.Web.UI.WebControls.WebParts.WebPartManager.CopyWebPart(System.Web.UI.WebControls.WebParts.WebPart)
additional_notes.overrides: *content
---

<p>The method is declared as `virtual` so that developers could inherit from the <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> class, override the method, and provide for additional scenarios in which it could create copies of controls. For example, the method could optionally receive as input a control that has been serialized into an XML file. The method could deserialize the XML (if present), and then call the base method to handle the existing cases and to return a new instance of a <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref> control.</p>


