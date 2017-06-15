---
uid: System.Data.Common.DbDataAdapter.GetBatchedParameter(System.Int32,System.Int32)
additional_notes.overrides: *content
---

<p>This method is protected and is designed for use by a .NET Framework data provider.  
  
 If a class that inherits from <xref href="System.Data.Common.DbDataAdapter"></xref> supports batches, that class overrides this method to allow users to execute a batch. An implementation uses the <code>commandIdentifier</code> provided to locate the requested command, then uses the <code>parameterIndex</code> provided to locate the requested parameter. For example, a <code>commandIdentifier</code> of 0 and a <code>parameterIndex</code> of 0 returns the first parameter from the first command in the batch.</p>


