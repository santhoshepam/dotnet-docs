---
uid: System.Web.UI.WebControls.WebParts.Part
additional_notes.overrides: *content
---

<p>Normally, you should not inherit directly from the <xref href="System.Web.UI.WebControls.WebParts.Part"></xref> class to develop custom Web Parts controls. To provide full Web Parts functionality, the Web Parts control set requires the classes derived from the <xref href="System.Web.UI.WebControls.WebParts.Part"></xref> class, namely <xref href="System.Web.UI.WebControls.WebParts.WebPart"></xref>, <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref>, and <xref href="System.Web.UI.WebControls.WebParts.CatalogPart"></xref>, so you should derive from them to develop custom controls. However, it is still important to understand the behavior of the base <xref href="System.Web.UI.WebControls.WebParts.Part"></xref> class, because it provides a common set of properties used by all other part classes.</p>


