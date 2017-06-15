---
uid: System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter"></xref> class, name your adapter for a given control type and markup language in the pattern <code>MarkupControlType</code>`Adapter` (for example, <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlTextBoxAdapter"></xref>). Adapters for a control that provides XHTML markup should be implemented in the <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters"></xref> namespace.  
  
 Any specialized adapters should be defined for the specialized control under each of the device nodes in the configuration .browser files.  
  
 A properly implemented control should not assume that an adapter is attached, or that the attached adapter implements a specific interface. Instead, it should check for these conditions.  
  
 A number of conditional rendering methods allow for such conditions as secondary UI and for display devices that require line breaks after every block or after every inline control. Examples of these conditional methods are <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter.ConditionalSetPendingBreak(System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlMobileTextWriter)"></xref> and <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter.ConditionalEnterLayout(System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlMobileTextWriter,System.Web.UI.MobileControls.Style)"></xref>. These methods work for a given device regardless of the control being rendered. It is unlikely you would need to override these methods when creating a new control adapter based on this class. At a minimum, you would need to override the <xref href="System.Web.UI.MobileControls.Adapters.XhtmlAdapters.XhtmlControlAdapter.Render*"></xref> methods.  
  
 Device filtering is required to use a specific adapter for a server control. For more information about device filtering, see [Architectural Overview of Adaptive Control Behavior](http://msdn.microsoft.com/library/4ff05ae9-4109-4352-929e-ad893895dbff) and [Device Filtering Overview](http://msdn.microsoft.com/library/bdfeaa58-dedd-4c0d-8610-988aac0eff19).</p>


