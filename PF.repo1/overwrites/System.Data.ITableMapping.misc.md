---
uid: System.Data.ITableMapping
additional_notes.overrides: *content
---

<p>When you inherit from the <xref href="System.Data.ITableMapping"></xref> interface, you should implement the following constructors:  
  
 <table><thead><tr><th> Item  
  
 </th><th> Description  
  
 </th></tr></thead><tbody><tr><td> DataTableMapping()  
  
 </td><td> Initializes a new instance of the TableMapping class.  
  
 </td></tr><tr><td> TableMapping(string sourceTable, string dataSetTable)  
  
 </td><td> Initializes a new instance of the TableMapping class with a source when given a source table name and a <xref href="System.Data.DataTable"></xref> name.  
  
 </td></tr><tr><td> TableMapping(string sourceTable, string dataSetTable, DataColumnMapping[] columnMappings)  
  
 </td><td> Initializes a new instance of the TableMapping class when given a source table name, a <xref href="System.Data.DataTable"></xref> name, and an array of ColumnMapping objects.  
  
 </td></tr></tbody></table></p>


