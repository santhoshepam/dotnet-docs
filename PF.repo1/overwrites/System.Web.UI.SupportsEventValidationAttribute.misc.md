---
uid: System.Web.UI.SupportsEventValidationAttribute
additional_notes.overrides: *content
---

<p>If you do not define the <xref href="System.Web.UI.SupportsEventValidationAttribute"></xref> attribute, your custom control does not automatically participate in event validation. However, your control can explicitly call <xref href="System.Web.UI.ClientScriptManager.ValidateEvent(System.String)"></xref>. If you handle event registration and validation, call <xref href="System.Web.UI.ClientScriptManager.ValidateEvent(System.String)"></xref>, and then you do not need to define this attribute on the control.</p>


