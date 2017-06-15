---
uid: System.Security.Permissions.ResourcePermissionBase
additional_notes.overrides: *content
---

<p>When you inherit from <xref href="System.Security.Permissions.ResourcePermissionBase"></xref>, you must provide at least three constructors, set two properties, and provide a third property. The required constructors are: a default constructor, one that takes a <xref href="System.Security.Permissions.PermissionState"></xref> as a parameter, and as many as needed that take values for the properties. The properties that need to be set are <xref href="System.Security.Permissions.ResourcePermissionBase.PermissionAccessType"></xref> and <xref href="System.Security.Permissions.ResourcePermissionBase.TagNames"></xref>. The third property that is needed is one that returns the permission entries. For an example of an implementation of this class, see <xref href="System.Diagnostics.PerformanceCounterPermission"></xref>. In <xref href="System.Diagnostics.PerformanceCounterPermission"></xref>, the <xref href="System.Security.Permissions.ResourcePermissionBase.TagNames"></xref> property is set privately to "Machine" and "Category", the <xref href="System.Security.Permissions.ResourcePermissionBase.PermissionAccessType"></xref> property is privately set to the type of <xref href="System.Diagnostics.PerformanceCounterPermissionAccess"></xref>, and the <xref href="System.Diagnostics.PerformanceCounterPermission.PermissionEntries"></xref> property returns the permission entries.</p>


