---
uid: System.Web.UI.WebControls.WebParts.WebZone
additional_notes.overrides: *content
---

<p>You rarely need to inherit directly from the <xref href="System.Web.UI.WebControls.WebParts.WebZone"></xref> class to develop custom Web Parts zones. The Web Parts control set contains the specialized zones listed above in the Remarks section, and usually you can derive from one of them to add custom behavior to a zone. If you do decide to inherit directly from the <xref href="System.Web.UI.WebControls.WebParts.WebZone"></xref> class, you must override a number of properties and methods (see the documentation for the members of the <xref href="System.Web.UI.WebControls.WebParts.WebZone"></xref> class). You must also create a custom <xref href="System.Web.UI.WebControls.WebParts.WebPartManager"></xref> control, optionally a custom <xref href="System.Web.UI.WebControls.WebParts.WebPartDisplayMode"></xref> control to create a unique display mode in which to view your zone, and other customizations to make your zone work within the Web Parts control set.</p>


