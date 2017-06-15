---
uid: System.Configuration.ConfigurationManager
additional_notes.overrides: *content
---

<p>The <xref href="System.Configuration.Configuration"></xref> class enables programmatic access for editing configuration files. You use one of the Open methods provided by <xref href="System.Configuration.ConfigurationManager"></xref>. These methods return a <xref href="System.Configuration.Configuration"></xref> object, which in turn provides the required methods and properties to handle the underlying configuration files. You can access these files for reading or writing.  
  
 To read the configuration files, use <xref href="System.Configuration.Configuration.GetSection(System.String)"></xref> or <xref href="System.Configuration.Configuration.GetSectionGroup(System.String)"></xref> to read configuration information. The user or process that reads must have the following permissions:  
  
-   Read permission on the configuration file at the current configuration hierarchy level.  
  
-   Read permissions on all the parent configuration files.  
  
 If your application needs read-only access to its own configuration, we recommend that you use the <xref href="System.Configuration.ConfigurationManager.GetSection(System.String)"></xref> method. This method provides access to the cached configuration values for the current application, which has better performance than the <xref href="System.Configuration.Configuration"></xref> class.  
  
 To write to the configuration files, use one of the <xref href="System.Configuration.Configuration.Save*"></xref> methods. The user or process that writes must have the following permissions:  
  
-   Write permission on the configuration file and directory at the current configuration hierarchy level.  
  
-   Read permissions on all the configuration files.</p>


