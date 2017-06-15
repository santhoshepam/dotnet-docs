---
summary: Sets the security descriptor for this <xref href="System.Security.AccessControl.ObjectSecurity"></xref> object from the specified Security Descriptor Definition Language (SDDL) string.
remarks: "If the security descriptor represented by the SDDL string contains `null` for its discretionary access control list (DACL), a single access control entry (ACE) that allows everyone full access (AEFA) is added to the DACL. If an application modifies the DACL of a security descriptor to which an AEFA ACE has been added, the AEFA ACE is persisted with the DACL when that DACL is persisted.  \n  \n This can result in an application unintentionally allowing access to principals. Because of this, an application should check for the existence of an AEFA ACE and remove it before modifying any security descriptor."
uid: System.Security.AccessControl.ObjectSecurity.SetSecurityDescriptorSddlForm*
---
