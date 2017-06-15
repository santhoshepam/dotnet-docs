---
summary: When overridden in a derived class, writes a restart area to the <xref href="System.IO.Log.IRecordSequence"></xref>.
remarks: A restart area is used to temporarily store information containing a client's last checkpoint operation. When a recovery is necessary, you can parse the restart area to retrieve all the data from the last checkpoint operation. This data initializes the transaction table, dirty pages table, and open file table so they can be used in the recovery process. A restart area can be read using the <xref:System.IO.Log.IRecordSequence.ReadRestartAreas%2A> method.
uid: System.IO.Log.IRecordSequence.WriteRestartArea*
---
