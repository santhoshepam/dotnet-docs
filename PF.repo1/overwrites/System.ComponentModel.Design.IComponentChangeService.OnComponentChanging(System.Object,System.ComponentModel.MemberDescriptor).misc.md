---
uid: System.ComponentModel.Design.IComponentChangeService.OnComponentChanging(System.Object,System.ComponentModel.MemberDescriptor)
additional_notes.overrides: *content
---

<p>This method throws an exception if the property cannot be changed. This is not intended to validate the values of a particular property. Instead, it is intended to provide a global method of preventing a component from changing. For example, if a designer file is checked into source code control, this event's handler would typically throw an exception if the user refused to check out the file.</p>


