---
uid: System.Data.IDataParameter
additional_notes.overrides: *content
---

<p>To promote consistency among .NET Framework data providers, name the inheriting class in the form <code>Prv</code> Parameter where <code>Prv</code> is the uniform prefix given to all classes in a specific .NET Framework data provider namespace. For example, <code>Sql</code> is the prefix of the <xref href="System.Data.SqlClient.SqlCommand"></xref> class in the `System.Data.SqlClient` namespace.  
  
 When you inherit from the <xref href="System.Data.IDataParameter"></xref> interface, you should implement the following constructors:  
  
 <table><thead><tr><th> Item  
  
 </th><th> Description  
  
 </th></tr></thead><tbody><tr><td> PrvParameter()  
  
 </td><td> Initializes a new instance of the Parameter class.  
  
 </td></tr><tr><td> PrvParameter(string name, PrvDbType dataType)  
  
 </td><td> Initializes a new instance of the Parameter class with the parameter name and data type.  
  
 </td></tr><tr><td> PrvParameter(string name, object value)  
  
 </td><td> Initializes a new instance of the Parameter class with the parameter name and an object that is the value of the Parameter.  
  
 </td></tr><tr><td> PrvParameter(string name, PrvDbType dataType, int size)  
  
 </td><td> Initializes a new instance of the Parameter class with the parameter name, data type, and width.  
  
 </td></tr><tr><td> PrvParameter(string name, PrvDbType dataType, int size, string srcColumn)  
  
 </td><td> Initializes a new instance of the DbParameter class with the parameter name, data type, width, and source column name.  
  
 </td></tr><tr><td> PrvParameter(string parameterName, PrvDbType dbType, int size, ParameterDirection direction, Boolean isNullable, Byte precision, Byte scale, string srcColumn, DataRowVersion srcVersion, object value)  
  
 </td><td> Initializes a new instance of the <xref href="System.Data.OleDb.OleDbParameter"></xref> class with the parameter name, data type, width, source column name, parameter direction, numeric precision, and other properties.  
  
 </td></tr></tbody></table></p>


