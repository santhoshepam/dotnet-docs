---
uid: System.Configuration.ConfigurationSection
additional_notes.overrides: *content
---

<p>You can use a programmatic or a declarative (attributed) coding model to create custom configuration sections:  
  
-   Programmatic model. This model requires that for each section attribute you create a property to get or set its value and add it to the internal property bag of the underlying <xref href="System.Configuration.ConfigurationElement"></xref> base class.  
  
-   Declarative model. This simpler model, also called the attributed model, allows you to define a section attribute by using a property and decorating it with attributes. These attributes instruct the ASP.NET configuration system about the property types and their default values. With this information, obtained through reflection, the ASP.NET configuration system creates the section property objects and performs the required initialization.  
  
 The <xref href="System.Configuration.Configuration"></xref> class allows programmatic access for editing configuration files. You can access these files for reading or writing as follows:  
  
-   Reading. You use <xref href="System.Configuration.Configuration.GetSection(System.String)"></xref> or <xref href="System.Configuration.Configuration.GetSectionGroup(System.String)"></xref> to read configuration information. Note that the user or process that reads must have the following permissions:  
  
    -   Read permission on the configuration file at the current configuration hierarchy level.  
  
    -   Read permissions on all the parent configuration files.  
  
     If your application needs read-only access to its own configuration, it is recommended you use the <xref href="System.Web.Configuration.WebConfigurationManager.GetSection*"></xref> overloaded methods in the case of Web applications, or the <xref href="System.Configuration.ConfigurationManager.GetSection(System.String)"></xref> method in the case of client applications.  
  
     These methods provide access to the cached configuration values for the current application, which has better performance than the <xref href="System.Configuration.Configuration"></xref> class.  
  
 <block subset="none" type="note"><p>  
 If you use a static `GetSection` method that takes a <code>path</code> parameter, the <code>path</code> parameter must refer to the application in which the code is running; otherwise, the parameter is ignored and configuration information for the currently-running application is returned.  
  
</p></block>  
  
-   Writing. You use one of the <xref href="System.Configuration.Configuration.Save*"></xref> methods to write configuration information. Note that the user or process that writes must have the following permissions:  
  
    -   Write permission on the configuration file and directory at the current configuration hierarchy level.  
  
    -   Read permissions on all the configuration files.</p>


