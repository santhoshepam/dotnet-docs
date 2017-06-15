---
uid: System.Web.UI.WebControls.WebParts.IWebEditable.CreateEditorParts
additional_notes.overrides: *content
---

<p>The <xref href="System.Web.UI.WebControls.WebParts.EditorPartCollection"></xref> object that the <xref href="System.Web.UI.WebControls.WebParts.IWebEditable.CreateEditorParts"></xref> method returns is read-only and has no accessible method to add individual controls to it. However, in your override or implementation of the method, you can create another kind of <xref href="System.Collections.ICollection"></xref> object, such as an <xref href="System.Collections.ArrayList"></xref>, to contain all the custom <xref href="System.Web.UI.WebControls.WebParts.EditorPart"></xref> controls, and pass it to the constructor when you create a new <xref href="System.Web.UI.WebControls.WebParts.EditorPartCollection"></xref> object. For a code example, see the Example section.</p>


