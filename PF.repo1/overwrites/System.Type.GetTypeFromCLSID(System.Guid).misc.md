---
uid: System.Type.GetTypeFromCLSID(System.Guid)
additional_notes.usage: *content
---

<p>This method is intended for use when working with COM objects, not with .NET Framework objects. All managed objects, including those that are visible to COM (that is, their <xref href="System.Runtime.InteropServices.ComVisibleAttribute"></xref> attribute is `true`) have a GUID that is returned by the <xref href="System.Type.GUID"></xref> property. Although the method returns a <xref href="System.Type"></xref> object that corresponds to the GUID for .NET Framework objects, you can't use that <xref href="System.Type"></xref> object to create a type instance by calling the  <xref href="System.Activator.CreateInstance(System.Type)"></xref> method, as the following example shows.  
  
 [!code-csharp[System.Type.GetTypeFromCLSID#11](~/samples/snippets/csharp/VS_Snippets_CLR_System/system.type.gettypefromclsid/cs/gettypefromclsid11.cs#11)]
 [!code-vb[System.Type.GetTypeFromCLSID#11](~/samples/snippets/visualbasic/VS_Snippets_CLR_System/system.type.gettypefromclsid/vb/gettypefromclsid11.vb#11)]  
  
 Instead, the <xref href="System.Type.GetTypeFromCLSID(System.Guid,System.String,System.Boolean)"></xref> should only be used to retrieve the GUID of an unmanaged COM object, and the resulting <xref href="System.Type"></xref> object that is passed to the <xref href="System.Activator.CreateInstance(System.Type)"></xref> method must represent an unmanaged COM object.</p>


