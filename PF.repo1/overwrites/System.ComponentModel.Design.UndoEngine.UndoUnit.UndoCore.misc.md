---
uid: System.ComponentModel.Design.UndoEngine.UndoUnit.UndoCore
additional_notes.overrides: *content
---

<p>Do not call the <xref href="System.ComponentModel.Design.UndoEngine.UndoUnit.UndoCore"></xref> method directly; override it if you want, but always call the `public`<xref href="System.ComponentModel.Design.UndoEngine.UndoUnit.Undo"></xref> method to perform undo work. The <xref href="System.ComponentModel.Design.UndoEngine.UndoUnit.Undo"></xref> method notifies the undo engine to suspend undo-operation data gathering until the current undo operation is completed. This prevents new undo units from being created in response to this unit doing work.</p>


