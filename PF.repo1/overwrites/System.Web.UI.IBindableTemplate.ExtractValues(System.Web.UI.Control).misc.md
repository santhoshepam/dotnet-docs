---
uid: System.Web.UI.IBindableTemplate.ExtractValues(System.Web.UI.Control)
additional_notes.overrides: *content
---

<p>An <xref href="System.Web.UI.IBindableTemplate.ExtractValues(System.Web.UI.Control)"></xref> method must conform to the following rules:  
  
-   If more than one binding exists for a given field, the last binding encountered is used.  
  
-   In order to reference a control's identifier in the <xref href="System.Web.UI.IBindableTemplate.ExtractValues(System.Web.UI.Control)"></xref> method, the control must also have a user-defined ID property at parse time. If no ID exists, this results in a parse error.  
  
-   Two-way ASP.NET data-binding syntax is only valid in an <xref href="System.Web.UI.ITemplate"></xref> or <xref href="System.Web.UI.IBindableTemplate"></xref> property of a data-bound control.</p>


