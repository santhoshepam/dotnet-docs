---
uid: System.Diagnostics.TraceListener.Write(System.String)
additional_notes.overrides: *content
---

<p>When inheriting from this class, you must implement this method. To support an indentation, you should call <xref href="System.Diagnostics.TraceListener.WriteIndent"></xref> if <xref href="System.Diagnostics.TraceListener.NeedIndent"></xref> is `true`. If you need to indent the following line, you must reset <xref href="System.Diagnostics.TraceListener.NeedIndent"></xref> to `true`.</p>


