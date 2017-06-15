---
uid: System.Windows.Forms.Control.DoubleClick
additional_notes.overrides: *content
---

<p>Inheriting from a standard Windows Forms control and changing the `StandardClick` or `StandardDoubleClick` values of <xref href="System.Windows.Forms.ControlStyles"></xref> to `true` can cause unexpected behavior or have no effect at all if the control does not support the <xref href="System.Windows.Forms.Control.Click"></xref> or <xref href="System.Windows.Forms.Control.DoubleClick"></xref> events.  
  
 The following table lists Windows Forms controls and which event (<xref href="System.Windows.Forms.Control.Click"></xref> or <xref href="System.Windows.Forms.Control.DoubleClick"></xref>) is raised in response to the mouse action specified.  
  
 <table><thead><tr><th> Control  
  
 </th><th> Left Mouse Click  
  
  Left Mouse Double Click  
  
  Right Mouse Click  
  
  Right Mouse Double Click  
  
  Middle Mouse Click  
  
  Middle Mouse Double Click  
  
  XButton1 Mouse Click  
  
  XButton1 Mouse Double-Click  
  
  XButton2 Mouse Click  
  
  XButton2 Mouse Double-Click  
  
 </th></tr></thead><tbody><tr><td><xref href="System.Windows.Forms.MonthCalendar"></xref>,  
  
 <xref href="System.Windows.Forms.DateTimePicker"></xref>,  
  
 <xref href="System.Windows.Forms.RichTextBox"></xref>,  
  
 <xref href="System.Windows.Forms.HScrollBar"></xref>,  
  
 <xref href="System.Windows.Forms.VScrollBar"></xref></td><td> none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
 </td></tr><tr><td><xref href="System.Windows.Forms.Button"></xref>,  
  
 <xref href="System.Windows.Forms.CheckBox"></xref>,  
  
 <xref href="System.Windows.Forms.RadioButton"></xref></td><td> Click  
  
  Click, Click  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
 </td></tr><tr><td><xref href="System.Windows.Forms.ListBox"></xref>,  
  
 <xref href="System.Windows.Forms.CheckedListBox"></xref>,  
  
 <xref href="System.Windows.Forms.ComboBox"></xref></td><td> Click  
  
  Click, DoubleClick  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
 </td></tr><tr><td><xref href="System.Windows.Forms.TextBox"></xref>,  
  
 <xref href="System.Windows.Forms.DomainUpDown"></xref>,  
  
 <xref href="System.Windows.Forms.NumericUpDown"></xref></td><td> Click  
  
  Click, DoubleClick  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
 </td></tr><tr><td> * <xref href="System.Windows.Forms.TreeView"></xref>,  
  
 \* <xref href="System.Windows.Forms.ListView"></xref></td><td> Click  
  
  Click, DoubleClick  
  
  Click  
  
  Click, DoubleClick  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
  none  
  
 </td></tr><tr><td><xref href="System.Windows.Forms.ProgressBar"></xref>,  
  
 <xref href="System.Windows.Forms.TrackBar"></xref></td><td> Click  
  
  Click, Click  
  
  Click  
  
  Click, Click  
  
  Click  
  
  Click, Click  
  
  Click  
  
  Click, Click  
  
  Click  
  
  Click, Click  
  
 </td></tr><tr><td><xref href="System.Windows.Forms.Form"></xref>,  
  
 <xref href="System.Windows.Forms.DataGrid"></xref>,  
  
 <xref href="System.Windows.Forms.Label"></xref>,  
  
 <xref href="System.Windows.Forms.LinkLabel"></xref>,  
  
 <xref href="System.Windows.Forms.Panel"></xref>,  
  
 <xref href="System.Windows.Forms.GroupBox"></xref>,  
  
 <xref href="System.Windows.Forms.PictureBox"></xref>,  
  
 <xref href="System.Windows.Forms.Splitter"></xref>,  
  
 <xref href="System.Windows.Forms.StatusBar"></xref>,  
  
 <xref href="System.Windows.Forms.ToolBar"></xref>,  
  
 <xref href="System.Windows.Forms.TabPage"></xref>,  
  
 ** <xref href="System.Windows.Forms.TabControl"></xref></td><td> Click  
  
  Click, DoubleClick  
  
  Click  
  
  Click, DoubleClick  
  
  Click  
  
  Click, DoubleClick  
  
  Click  
  
  Click, DoubleClick  
  
  Click  
  
  Click, DoubleClick  
  
 </td></tr></tbody></table>  
  
 \* The mouse pointer must be over a child object (<xref href="System.Windows.Forms.TreeNode"></xref> or <xref href="System.Windows.Forms.ListViewItem"></xref>).  
  
 ** The <xref href="System.Windows.Forms.TabControl"></xref> must have at least one <xref href="System.Windows.Forms.TabPage"></xref> in its <xref href="System.Windows.Forms.TabControl.TabPages"></xref> collection.</p>


