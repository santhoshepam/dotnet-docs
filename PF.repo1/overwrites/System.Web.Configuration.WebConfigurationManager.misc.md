---
uid: System.Web.Configuration.WebConfigurationManager
additional_notes.overrides: *content
---

<p>The <xref href="System.Configuration.Configuration"></xref> class allows programmatic access for editing configuration files. You use one of the open methods provided by <xref href="System.Web.Configuration.WebConfigurationManager"></xref>. These methods will return a <xref href="System.Configuration.Configuration"></xref> object, which in turn provides the required methods and properties to handle the underlying configuration files. You can access these files for reading or writing as follows:  
  
 You use <xref href="System.Configuration.Configuration.GetSection(System.String)"></xref> or <xref href="System.Configuration.Configuration.GetSectionGroup(System.String)"></xref> to read configuration information. Note that the user or process that reads must have the following permissions:  
  
-   Read permission on the configuration file at the current configuration hierarchy level.  
  
-   Read permissions on all the parent configuration files.  
  
 If your application needs read-only access to its own configuration, it is recommended you use the <xref href="System.Web.Configuration.WebConfigurationManager.GetSection*"></xref> methods. These methods provide access to the cached configuration values for the current application, which has better performance than the <xref href="System.Configuration.Configuration"></xref> class.  
  
 <block subset="none" type="note"><p>  
 If you use a static `GetSection` method that takes a <code>path</code> parameter, the path parameter must refer to the application in which the code is running; otherwise, the parameter is ignored and configuration information for the currently-running application is returned.  
  
</p></block>  
  
 You use one of the <xref href="System.Configuration.Configuration.Save*"></xref> methods to write configuration information. Note that the user or process that writes must have the following permissions:  
  
-   Write permission on the configuration file and directory at the current configuration hierarchy level.  
  
-   Read permissions on all the configuration files.</p>


