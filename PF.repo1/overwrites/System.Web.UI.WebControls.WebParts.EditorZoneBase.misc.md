---
uid: System.Web.UI.WebControls.WebParts.EditorZoneBase
additional_notes.overrides: *content
---

<p>If you want to develop a custom zone for hosting <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> controls, you must determine whether you want to provide zone template support. A zone template is created by types that implement the <xref href="System.Web.UI.ITemplate"></xref> interface, and is necessary if you want to enable page developers using your custom zone to reference <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> controls within your zone in the declarative markup of a Web page. If you need zone template support, you should inherit from the <xref href="System.Web.UI.WebControls.WebParts.EditorZone"></xref> class.  
  
 In contrast, if your custom zone and its <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> controls are going to be self-contained, and they will be created programmatically without any options for page developers to specify controls declaratively in a zone template, then you can inherit directly from the <xref href="System.Web.UI.WebControls.WebParts.EditorZoneBase"></xref> class. If you do this, it is critical that you implement the <xref href="System.Web.UI.WebControls.WebParts.EditorZoneBase.CreateEditorParts"></xref> method so that your custom zone will work.</p>


