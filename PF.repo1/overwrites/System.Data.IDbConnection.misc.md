---
uid: System.Data.IDbConnection
additional_notes.overrides: *content
---

<p>To promote consistency among .NET Framework data providers, name the inheriting class in the form <code>PrvClassname</code> where <code>Prv</code> is the uniform prefix given to all classes in a specific .NET Framework data provider namespace. For example, <code>Sql</code> is the prefix of the <xref href="System.Data.SqlClient.SqlConnection"></xref> class in the `System.Data.SqlClient` namespace.  
  
 When you inherit from the <xref href="System.Data.IDbConnection"></xref> interface, you should implement the following constructors:  
  
 <table><thead><tr><th> Item  
  
 </th><th> Description  
  
 </th></tr></thead><tbody><tr><td> PrvConnection()  
  
 </td><td> Initializes a new instance of the PrvConnection class.  
  
 </td></tr><tr><td> PrvConnection(string connectionString)  
  
 </td><td> Initializes a new instance of the PrvConnection class when given a string containing the connection string.  
  
 </td></tr></tbody></table></p>


