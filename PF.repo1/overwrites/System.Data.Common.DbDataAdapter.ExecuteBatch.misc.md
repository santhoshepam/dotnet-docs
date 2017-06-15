---
uid: System.Data.Common.DbDataAdapter.ExecuteBatch
additional_notes.overrides: *content
---

<p>This method is protected and is designed for use by a .NET Framework data provider.  
  
 If a class that inherits from <xref href="System.Data.Common.DbDataAdapter"></xref> supports batches, that class overrides this method to allow users to execute a batch. An implementation of this method combines the commands in the adapter into a batch, then executes the batch and returns the return value of the batch.</p>


