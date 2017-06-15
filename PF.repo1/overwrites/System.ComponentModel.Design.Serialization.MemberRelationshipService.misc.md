---
uid: System.ComponentModel.Design.Serialization.MemberRelationshipService
additional_notes.overrides: *content
---

<p>The <xref href="System.ComponentModel.Design.Serialization.MemberRelationshipService"></xref> class is `abstract`. Implementing a concrete version varies depending on the types of members that are supported. For example, relating one event to another might require a different implementation than relating one property to another. Implementing the service requires the following steps:  
  
-   Implement <xref href="System.ComponentModel.Design.Serialization.MemberRelationshipService.SupportsRelationship(System.ComponentModel.Design.Serialization.MemberRelationship,System.ComponentModel.Design.Serialization.MemberRelationship)"></xref> to return `true` for relationships that you support.  
  
-   Track changes to the source relationship and assign value changes into the target relationship.</p>


