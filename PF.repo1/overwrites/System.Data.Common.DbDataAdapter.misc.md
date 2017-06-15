---
uid: System.Data.Common.DbDataAdapter
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Data.Common.DbDataAdapter"></xref> class, we recommend that you implement the following constructors:  
  
 <table><thead><tr><th> Item  
  
 </th><th> Description  
  
 </th></tr></thead><tbody><tr><td> *Prv*DataAdapter()  
  
 </td><td> Initializes a new instance of the *Prv*DataAdapter class.  
  
 </td></tr><tr><td> *Prv*DataAdapter(*Prv*Command *selectCommand*)  
  
 </td><td> Initializes a new instance of the *Prv*DataAdapter class with the specified SQL SELECT statement.  
  
 </td></tr><tr><td> *Prv*DataAdapter(string *selectCommandText*, string *selectConnectionString*)  
  
 </td><td> Initializes a new instance of the *Prv*DataAdapter class with an SQL SELECT statement and a connection string.  
  
 </td></tr><tr><td> *Prv*DataAdapter(string *selectCommandText*, *Prv*Connection *selectConnection*)  
  
 </td><td> Initializes a new instance of the *Prv*DataAdapter class with an SQL SELECT statement and a *Prv*Connection object.  
  
 </td></tr></tbody></table>  
  
 To promote consistency among .NET Framework data providers, you should name the inheriting class in the form *Prv*DataAdapter, where *Prv* is the uniform prefix given to all classes in a specific .NET Framework data provider namespace. For example, "Sql" is the prefix of the <xref href="System.Data.SqlClient.SqlDataAdapter"></xref> class in the **System.Data.SqlClient** namespace.</p>


