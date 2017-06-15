---
uid: System.Web.Profile.ProfileBase
additional_notes.overrides: *content
---

<p>You can create a custom profile implementation that inherits from the <xref href="System.Web.Profile.ProfileBase"></xref> abstract class and defines properties for the user profile that are not specified in the  configuration element. You can specify a custom user-profile type in the Web.config file with the `inherits` attribute of the  configuration element, as shown in the following example. The code for the <code>EmployeeProfile</code> class is included in the Example section of this topic.  
  
```  
<profile inherits="Samples.AspNet.Profile.EmployeeProfile"  
  defaultProvider="SqlProvider">  
  <providers>  
    <clear />  
    <add  
      name="SqlProvider"  
      type="System.Web.Profile.SqlProfileProvider"   
      connectionStringName="SqlServices"   
      description="SQL Profile Provider for Sample"/>   
    <add  
      name="EmployeeInfoProvider"  
      type="System.Web.Profile.SqlProfileProvider"   
      connectionStringName="SqlServices"   
      description="SQL Profile Provider for Employee Info"/>   
  </providers>  
  
  <properties>  
    <add name="GarmentSize" />  
  </properties>  
</profile>  
```</p>


