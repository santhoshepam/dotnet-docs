---
uid: System.Web.UI.WebControls.WebParts.ToolZone
additional_notes.overrides: *content
---

<p>The Web Parts control set contains the specialized zones listed above in the Remarks section, and you can often derive from one of them to add custom behavior to a zone. However, for more programmatic control over the rendering of a zone, you should inherit directly from the <xref href="System.Web.UI.WebControls.WebParts.ToolZone"></xref> class. For example, you might want to create a custom zone for a specialized task, such as a search zone.  
  
 To create a custom zone, you can override any of the virtual <xref href="System.Web.UI.WebControls.WebParts.ToolZone"></xref> members to fully customize the rendering, or you can override only a specific member. Optionally, you can also create a custom display mode for your zone by inheriting from the <xref href="System.Web.UI.WebControls.WebParts.WebPartDisplayMode"></xref> class, but this is not required. In the constructor of your zone, you should add the various display modes in which you want your zone to be displayed to a <xref href="System.Web.UI.WebControls.WebParts.WebPartDisplayModeCollection"></xref> object, so that your zone is visible when the page is in those display modes.</p>


