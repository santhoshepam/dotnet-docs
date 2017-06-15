---
summary: Copies all rows from a data source to a destination table specified by the <xref href="System.Data.SqlClient.SqlBulkCopy.DestinationTableName"></xref> property of the <xref href="System.Data.SqlClient.SqlBulkCopy"></xref> object.
remarks: If multiple active result sets (MARS) is disabled, <xref:System.Data.SqlClient.SqlBulkCopy.WriteToServer%2A> makes the connection busy. If MARS is enabled, you can interleave calls to <xref:System.Data.SqlClient.SqlBulkCopy.WriteToServer%2A> with other commands in the same connection.
uid: System.Data.SqlClient.SqlBulkCopy.WriteToServer*
---
