---
uid: System.Windows.Forms.Control.ProcessKeyMessage(System.Windows.Forms.Message@)
additional_notes.overrides: *content
---

<p>When overriding the <xref href="System.Windows.Forms.Control.ProcessKeyMessage(System.Windows.Forms.Message@)"></xref> method, a control should return `true` to indicate that it has processed the key. For keys that are not processed by the control, the result of the base class's <xref href="System.Windows.Forms.Control.ProcessKeyEventArgs(System.Windows.Forms.Message@)"></xref> should be returned. Controls will seldom, if ever, need to override this method.</p>


