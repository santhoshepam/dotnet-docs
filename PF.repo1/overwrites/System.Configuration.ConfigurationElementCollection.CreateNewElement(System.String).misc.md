---
uid: System.Configuration.ConfigurationElementCollection.CreateNewElement(System.String)
additional_notes.overrides: *content
---

<p>If you create a custom <xref href="System.Configuration.ConfigurationElementCollection"></xref> collection that contains heterogeneous <xref href="System.Configuration.ConfigurationElement"></xref> types, you must perform these steps:  
  
-   Override the <xref href="System.Configuration.ConfigurationElementCollection.GetElementKey(System.Configuration.ConfigurationElement)"></xref> method.  
  
-   Make sure that the <xref href="System.Configuration.ConfigurationElementCollection.GetElementKey(System.Configuration.ConfigurationElement)"></xref> method returns a string that identifies the type of the element you created by calling the <xref href="System.Configuration.ConfigurationElementCollection.CreateNewElement(System.String)"></xref> method.</p>


