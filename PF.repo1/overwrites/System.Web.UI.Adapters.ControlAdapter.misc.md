---
uid: System.Web.UI.Adapters.ControlAdapter
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Web.UI.Adapters.ControlAdapter"></xref> class, a control that requires general adapter functionality should have a corresponding adapter base class, named in the pattern <code>ControlType</code>`Adapter` (for example, `TextBoxAdapter`). The adapter should at a minimum return a strongly-typed instance of the control through its <xref href="System.Web.UI.Adapters.ControlAdapter.Control"></xref> property.  
  
1.  Control adapters for a given control type and markup language should be named in the pattern <code>MarkupControlType</code>`Adapter` (for example, `XhtmlTextBoxAdapter`). Adapters for a control should be implemented in an `Adapters` subnamespace.  
  
 Control adapters should inherit from the appropriate base class and follow the same inheritance model as the control. For example, an adapter for a control inheriting from the <xref href="System.Web.UI.Control"></xref> base class should inherit from either the <xref href="System.Web.UI.Adapters.ControlAdapter"></xref> class or the relevant <code>ControlType</code>`Adapter` class.  
  
 Any specialized adapters should be defined for the specialized control under all of the device nodes in configuration .browser files.  
  
 A properly implemented control should not assume that an adapter is attached, or that the attached adapter implements a specific interface. Instead, it should check for these before calling.  
  
 It is possible to simulate overriding protected event methods in the control, such as the <xref href="System.Web.UI.WebControls.LinkButton.OnClick(System.EventArgs)"></xref> method of the <xref href="System.Web.UI.WebControls.LinkButton"></xref>. First, create an adapter class with an <code>OnClick</code> method. Then create a new control derived from <xref href="System.Web.UI.WebControls.LinkButton"></xref> and override the <xref href="System.Web.UI.WebControls.LinkButton.OnClick(System.EventArgs)"></xref> method. The overriden <xref href="System.Web.UI.WebControls.LinkButton.OnClick(System.EventArgs)"></xref> method calls the <code>OnClick</code> method of the adapter. The adapter object is available through the protected <xref href="System.Web.UI.Control.Adapter"></xref> property of the <xref href="System.Web.UI.Control"></xref> class. The <xref href="System.Web.UI.Control.Adapter"></xref> property of the control is `null` when there is no associated adapter, so any code should check for that condition before calling methods of the adapter.</p>


