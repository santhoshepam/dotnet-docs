---
summary: Loads a <xref href="System.Web.UI.Control"></xref>.
remarks: When you load a control into a container control, the container raises all of the added control's events until it has caught up to the current event. However, the added control does not catch up with postback data processing. For an added control to participate in postback data processing, including validation, the control must be added in the <xref:System.Web.UI.Control.Init> event rather than in the <xref:System.Web.UI.Control.Load> event.
uid: System.Web.UI.TemplateControl.LoadControl*
---
