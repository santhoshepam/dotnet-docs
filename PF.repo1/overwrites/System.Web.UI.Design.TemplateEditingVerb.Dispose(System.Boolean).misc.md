---
uid: System.Web.UI.Design.TemplateEditingVerb.Dispose(System.Boolean)
additional_notes.overrides: *content
---

<p>
      <block subset="none" type="note">
        <p>  
 The <xref href="System.Web.UI.Design.TemplateEditingVerb"></xref> class is obsolete. Expose templates through the <xref href="System.Web.UI.Design.ControlDesigner.TemplateGroups"></xref> property of a control designer. The design host creates a <xref href="System.Web.UI.Design.TemplatedEditableDesignerRegion"></xref> for each <xref href="System.Web.UI.Design.TemplateGroup"></xref> defined for a control designer.  
  
</p>
      </block>
      `Dispose` can be called multiple times by other objects. When overriding `Dispose(Boolean)`, be careful not to reference objects that have been previously disposed of in an earlier call to `Dispose`. For more information about how to implement `Dispose(Boolean)`, see [Implementing a Dispose Method](~/docs/standard/garbage-collection/implementing-dispose.md).  
  
 For more information about `Dispose` and <xref href="System.Object.Finalize"></xref>, see [Cleaning Up Unmanaged Resources](~/docs/standard/garbage-collection/unmanaged.md) and [Overriding the Finalize Method](http://msdn.microsoft.com/en-us/8026cb68-fe93-43fc-96c1-c09ad7d64cd3).</p>


