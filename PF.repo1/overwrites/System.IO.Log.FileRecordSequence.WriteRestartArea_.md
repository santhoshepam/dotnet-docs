---
summary: Writes a restart area to the <xref href="System.IO.Log.FileRecordSequence"></xref>.
remarks: "A restart area can be used to temporarily store information containing a client's last checkpoint operation. When a recovery is necessary, you can read a restart area and retrieve all the data from the last checkpoint operation. This data initializes the transaction table, dirty pages table, and open file table so they can be used in the recovery process.  \n  \n A restart area can be read using the <xref:System.IO.Log.FileRecordSequence.ReadRestartAreas%2A> method."
uid: System.IO.Log.FileRecordSequence.WriteRestartArea*
---
