---
uid: System.ComponentModel.PropertyDescriptor.SetValue(System.Object,System.Object)
additional_notes.overrides: *content
---

<p>When you override this method, it should set the value of the property by invoking the appropriate "SetMyProperty" method that you need to implement. If the value specified is not valid, the component should throw an exception, which is passed up. You should design the property so that a "GetMyProperty" method (that you have implemented) following a "SetMyProperty" method returns the value passed in when the "SetMyProperty" method does not throw an exception.</p>


