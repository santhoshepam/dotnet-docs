---
uid: System.Windows.Forms.ContextMenu.ProcessCmdKey(System.Windows.Forms.Message@,System.Windows.Forms.Keys,System.Windows.Forms.Control)
additional_notes.overrides: *content
---

<p>When overriding the <xref href="System.Windows.Forms.Control.ProcessCmdKey(System.Windows.Forms.Message@,System.Windows.Forms.Keys)"></xref> method in a derived class, a control should return `true` to indicate that it has processed the key. For keys that are not processed by the control, the result of calling the base class's <xref href="System.Windows.Forms.Control.ProcessCmdKey(System.Windows.Forms.Message@,System.Windows.Forms.Keys)"></xref> method should be returned. Controls will seldom, if ever, need to override this method.</p>


