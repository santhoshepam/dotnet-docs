---
uid: System.Windows.Forms.Control
thread_safety: *content
---

Only the following members are thread safe: <xref href="System.Windows.Forms.Control.BeginInvoke(System.Delegate)"></xref>, <xref href="System.Windows.Forms.Control.EndInvoke(System.IAsyncResult)"></xref>, <xref href="System.Windows.Forms.Control.Invoke(System.Delegate)"></xref>, <xref href="System.Windows.Forms.Control.InvokeRequired"></xref>, and <xref href="System.Windows.Forms.Control.CreateGraphics"></xref> if the handle for the control has already been created. Calling <xref href="System.Windows.Forms.Control.CreateGraphics"></xref> before the control's handle has been created on a background thread can cause illegal cross thread calls.


