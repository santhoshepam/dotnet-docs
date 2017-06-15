---
summary: Sends results directly to the client or current output consumer.
remarks: The **Send** method sends data straight to the client or caller. It is usually the client that consumes the output from the **Pipe** method, but in the case of nested CLR stored procedures the output consumer can also be a stored procedure. For example, Procedure1 calls <xref:System.Data.SqlClient.SqlCommand.ExecuteReader%2A> with the command text "EXEC Procedure2". Procedure2 is also a managed stored procedure. If Procedure2 now calls <xref:Microsoft.SqlServer.Server.SqlPipe.Send%2A>, the row is sent to Procedure1's reader, not to the client.
uid: Microsoft.SqlServer.Server.SqlPipe.Send*
---
