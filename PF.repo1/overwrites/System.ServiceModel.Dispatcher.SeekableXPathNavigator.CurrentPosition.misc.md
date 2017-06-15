---
uid: System.ServiceModel.Dispatcher.SeekableXPathNavigator.CurrentPosition
additional_notes.overrides: *content
---

<p>This property does not have any intrinsic meaning: it is an opaque <xref href="System.Int64"></xref> value that an implementation associates with the navigator’s current position. No restrictions or requirements are placed on the value itself. No assumptions about its internal data structure can be made.  
  
 It is not required that the values be sequential, or even that a navigator position map to a unique value. Multiple values can refer to the same navigator position, so comparing two values does not provide useful information.  
  
 Any value supplied by a `get` operation must be valid for a `set` operation. It is not necessarily an error for a `set` operation to use a value not first acquired by a `get` operation. A value not returned by <xref href="System.ServiceModel.Dispatcher.SeekableXPathNavigator.CurrentPosition"></xref> that has been acquired some other way may or may not be considered valid by the implementation: this choice is up to the implementer.  
  
 The meaning of a value must not change during the life of its navigator while it navigates the same document. Also, the meaning of values must be shared by any two navigators that are related by cloning, again, provided they still navigate the same document. All values supplied by a `get` operation must remain valid for the life of a navigator and any of its clones as long as the instance still navigates the same document.</p>


