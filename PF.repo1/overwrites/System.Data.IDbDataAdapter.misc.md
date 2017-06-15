---
uid: System.Data.IDbDataAdapter
additional_notes.overrides: *content
---

<p>To promote consistency among .NET Framework data providers, name the inheriting class in the form <code>Prv</code> DataAdapter where <code>Prv</code> is the uniform prefix given to all classes in a specific .NET Framework data provider namespace. For example, <code>Sql</code> is the prefix of the <xref href="System.Data.SqlClient.SqlDataAdapter"></xref> class in the `System.Data.SqlClient` namespace.  
  
 When you inherit from the <xref href="System.Data.IDbDataAdapter"></xref> interface, you should implement the following constructors:  
  
 <table><thead><tr><th> Item  
  
 </th><th> Description  
  
 </th></tr></thead><tbody><tr><td> PrvDataAdapter()  
  
 </td><td> Initializes a new instance of the PrvDataAdapter class.  
  
 </td></tr><tr><td> PrvDataAdapter(PrvCommand selectCommand)  
  
 </td><td> Initializes a new instance of the PrvDataAdapter class with the specified SQL SELECT statement.  
  
 </td></tr><tr><td> PrvDataAdapter(string selectCommandText, string selectConnectionString)  
  
 </td><td> Initializes a new instance of the PrvDataAdapter class with an SQL SELECT statement and a connection string.  
  
 </td></tr><tr><td> PrvDataAdapter(string selectCommandText, PrvConnection selectConnection)  
  
 </td><td> Initializes a new instance of the PrvDataAdapter class with an SQL SELECT statement and a PrvConnection object.  
  
 </td></tr></tbody></table></p>


