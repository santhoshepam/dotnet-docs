---
uid: System.Windows.Forms.Layout.LayoutEngine.Layout(System.Object,System.Windows.Forms.LayoutEventArgs)
additional_notes.overrides: *content
---

<p>Override the <xref href="System.Windows.Forms.Layout.LayoutEngine.Layout(System.Object,System.Windows.Forms.LayoutEventArgs)"></xref> method to provide your custom layout behavior.  
  
 When laying out the contents of the <code>container</code> parameter, be sure to check the <xref href="System.Windows.Forms.Control.Visible"></xref> property of each child control.  
  
 Return `true` if your layout engine logic determines that layout should be performed again by the parent of the container. This might occur, for example, when the layout engine resizes child controls and determines that the container must be increased in size to accommodate the new layout.</p>


