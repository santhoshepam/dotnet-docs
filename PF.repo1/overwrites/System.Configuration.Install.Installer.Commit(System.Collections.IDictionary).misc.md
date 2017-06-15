---
uid: System.Configuration.Install.Installer.Commit(System.Collections.IDictionary)
additional_notes.overrides: *content
---

<p>If you override the <xref href="System.Configuration.Install.Installer.Commit(System.Collections.IDictionary)"></xref> method in a derived class, be sure to call the base class's <xref href="System.Configuration.Install.Installer.Commit(System.Collections.IDictionary)"></xref> method first in your derived method. The <xref href="System.Configuration.Install.Installer.Commit(System.Collections.IDictionary)"></xref> method is called only if the <xref href="System.Configuration.Install.Installer.Install(System.Collections.IDictionary)"></xref> method of each installer in this instance's <xref href="System.Configuration.Install.InstallerCollection"></xref> succeeds. The <xref href="System.Configuration.Install.Installer.Commit(System.Collections.IDictionary)"></xref> method stores information needed to do a correct uninstallation, and calls the <xref href="System.Configuration.Install.Installer.Commit(System.Collections.IDictionary)"></xref> method of each installer in the collection.</p>


