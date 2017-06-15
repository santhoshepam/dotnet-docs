---
uid: System.Data.IDbCommand
additional_notes.overrides: *content
---

<p>To promote consistency among .NET Framework data providers, name the inheriting class in the form <code>PrvClassname</code> where <code>Prv</code> is the uniform prefix given to all classes in a specific .NET Framework data provider namespace. For example, <code>Sql</code> is the prefix of the <xref href="System.Data.SqlClient.SqlCommand"></xref> class in the `System.Data.SqlClient` namespace.  
  
 When you inherit from the <xref href="System.Data.IDbCommand"></xref> interface, you should implement the following constructors:  
  
 <table><thead><tr><th> Item  
  
 </th><th> Description  
  
 </th></tr></thead><tbody><tr><td> PrvCommand()  
  
 </td><td> Initializes a new instance of the PrvCommand class.  
  
 </td></tr><tr><td> PrvCommand(string cmdText)  
  
 </td><td> Initializes a new instance of the PrvCommand class with the text of the query.  
  
 </td></tr><tr><td> PrvCommand(string cmdText, PrvConnection connection)  
  
 </td><td> Initializes a new instance of the PrvCommand class with the text of the query and a PrvConnection.  
  
 </td></tr><tr><td> PrvCommand(string cmdText, PrvConnection connection, PrvTransaction transaction)  
  
 </td><td> Initializes a new instance of the PrvCommand class with the text of the query, a PrvConnection, and the PrvTransaction.  
  
 </td></tr></tbody></table></p>


