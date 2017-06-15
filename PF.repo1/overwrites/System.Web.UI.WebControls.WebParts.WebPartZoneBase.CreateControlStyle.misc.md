---
uid: System.Web.UI.WebControls.WebParts.WebPartZoneBase.CreateControlStyle
additional_notes.overrides: *content
---

<p>If you override the <xref href="System.Web.UI.WebControls.WebParts.WebPartZoneBase.CreateControlStyle"></xref> method to set some specific properties on the created style, do not use the <xref href="System.Web.UI.WebControls.Style.#ctor(System.Web.UI.StateBag)"></xref> version of the constructor, which requires you to pass the control's <xref href="System.Web.UI.StateBag"></xref> object in as a parameter, resulting in the created <xref href="System.Web.UI.WebControls.Style"></xref> object sharing the <xref href="System.Web.UI.StateBag"></xref> with the zone control. This causes rendering problems. Instead, use the <xref href="System.Web.UI.WebControls.Style.#ctor"></xref> version of the constructor, so the <xref href="System.Web.UI.WebControls.Style"></xref> object is independent of the control.</p>


