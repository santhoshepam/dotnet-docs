---
uid: System.Configuration.Configuration
additional_notes.overrides: *content
---

<p>The <xref href="System.Configuration.Configuration"></xref> class provides programmatic access for editing configuration files. You use one of the "Open" methods provided by the <xref href="System.Web.Configuration.WebConfigurationManager"></xref> class for Web applications or by the <xref href="System.Configuration.ConfigurationManager"></xref> class for client applications. These methods return a <xref href="System.Configuration.Configuration"></xref> object, which in turn provides the methods and properties that handle the underlying configuration files. You can access these files for reading or writing configuration information.  
  
 You use the <xref href="System.Configuration.Configuration.GetSection(System.String)"></xref> method or the <xref href="System.Configuration.Configuration.GetSectionGroup(System.String)"></xref> method to read configuration information. Note that the user or process that reads must have the following permissions:  
  
-   Read permission on the configuration file at the current configuration hierarchy level.  
  
-   Read permissions on all the parent configuration files.  
  
 If your application needs read-only access to its own configuration, it is recommended that you use the <xref href="System.Web.Configuration.WebConfigurationManager.GetSection*"></xref> method overloads for Web applications. For client application, use the <xref href="System.Configuration.ConfigurationManager.GetSection(System.String)"></xref> method.  
  
 These methods provide access to the cached configuration values for the current application, which has better performance than the <xref href="System.Configuration.Configuration"></xref> class.  
  
 <block subset="none" type="note"><p>  
 If you use a static `GetSection` method that takes a path parameter, the path parameter must refer to the application in which the code is running, otherwise the parameter is ignored and configuration information for the currently running application is returned.  
  
</p></block>  
  
 You use one of the <xref href="System.Configuration.Configuration.Save*"></xref> methods to write configuration information. Note that the user or process that writes must have the following permissions:  
  
-   Write permission on the configuration file and directory at the current configuration hierarchy level.  
  
-   Read permissions on all the configuration files.</p>


