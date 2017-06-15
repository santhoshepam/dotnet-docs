---
summary: Writes a restart area to the <xref href="System.IO.Log.LogRecordSequence"></xref>.
remarks: "A restart area is used to temporarily store information containing a client's last checkpoint operation. The Common Log File System (CLFS) maintains two restart areas to guarantee that at least one valid area is always available. When a recovery is necessary, the CLFS reads its restart area and all the data from the last checkpoint operation. This data initializes the transaction table, dirty pages table, and open file table so they can be used in the recovery process.  \n  \n A restart area can be read using the <xref:System.IO.Log.LogRecordSequence.ReadRestartAreas%2A> method."
uid: System.IO.Log.LogRecordSequence.WriteRestartArea*
---
