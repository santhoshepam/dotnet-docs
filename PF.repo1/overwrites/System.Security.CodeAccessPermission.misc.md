---
uid: System.Security.CodeAccessPermission
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.Security.CodeAccessPermission"></xref>, you must also implement the <xref href="System.Security.Permissions.IUnrestrictedPermission"></xref> interface.  
  
 The following <xref href="System.Security.CodeAccessPermission"></xref> members must be overridden: <xref href="System.Security.CodeAccessPermission.Copy"></xref>, <xref href="System.Security.CodeAccessPermission.Intersect(System.Security.IPermission)"></xref>, <xref href="System.Security.CodeAccessPermission.IsSubsetOf(System.Security.IPermission)"></xref>, <xref href="System.Security.CodeAccessPermission.ToXml"></xref>, <xref href="System.Security.CodeAccessPermission.FromXml(System.Security.SecurityElement)"></xref>, and <xref href="System.Security.CodeAccessPermission.Union(System.Security.IPermission)"></xref>.  
  
 You must also define a constructor that takes a <xref href="System.Security.Permissions.PermissionState"></xref> as its only parameter.  
  
 You must apply the <xref href="System.SerializableAttribute"></xref> attribute to a class that inherits from <xref href="System.Security.CodeAccessPermission"></xref>.</p>


