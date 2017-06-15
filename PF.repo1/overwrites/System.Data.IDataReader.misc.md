---
uid: System.Data.IDataReader
additional_notes.overrides: *content
---

<p>To promote consistency among .NET Framework data providers, name the inheriting class in the form <code>Prv</code> Command where <code>Prv</code> is the uniform prefix given to all classes in a specific .NET Framework data provider namespace. For example, <code>Sql</code> is the prefix of the <xref href="System.Data.SqlClient.SqlDataAdapter"></xref> class in the `System.Data.SqlClient` namespace.  
  
 Users do not create an instance of a `DataReader` class directly. Instead, they obtain the `DataReader` instance through the `ExecuteReader` method of the `Command` object. Therefore, you should mark `DataReader` constructors as internal.</p>


