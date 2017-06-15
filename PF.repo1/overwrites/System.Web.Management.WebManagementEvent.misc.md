---
uid: System.Web.Management.WebManagementEvent
additional_notes.overrides: *content
---

<p>When formatting your custom event information for display, override the <xref href="System.Web.Management.WebBaseEvent.FormatCustomEventDetails(System.Web.Management.WebEventFormatter)"></xref> method rather than the <xref href="System.Web.Management.WebBaseEvent.ToString*"></xref> method. This will avoid overwriting or tampering with sensitive system information.  
  
 The event code you specify for your custom event must be greater than <xref href="System.Web.Management.WebEventCodes.WebExtendedBase"></xref>.</p>


