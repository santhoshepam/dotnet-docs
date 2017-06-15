---
uid: System.ComponentModel.LicenseContext
additional_notes.overrides: *content
---

<p>If you want to implement design-time license support, you must inherit from this class, and override the following members: <xref href="System.ComponentModel.LicenseContext.UsageMode"></xref>, <xref href="System.ComponentModel.LicenseContext.GetSavedLicenseKey(System.Type,System.Reflection.Assembly)"></xref>, <xref href="System.ComponentModel.LicenseContext.GetService(System.Type)"></xref>, and <xref href="System.ComponentModel.LicenseContext.SetSavedLicenseKey(System.Type,System.String)"></xref>. If you want to implement saved license keys, override the <xref href="System.ComponentModel.LicenseContext.GetSavedLicenseKey(System.Type,System.Reflection.Assembly)"></xref> and <xref href="System.ComponentModel.LicenseContext.SetSavedLicenseKey(System.Type,System.String)"></xref> methods.  
  
 For more information about licensing, see [How to: License Components and Controls](http://msdn.microsoft.com/library/8e66c1ed-a445-4b26-8185-990b6e2bbd57).</p>


