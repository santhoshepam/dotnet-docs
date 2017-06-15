---
uid: System.Diagnostics.TraceFilter.ShouldTrace(System.Diagnostics.TraceEventCache,System.String,System.Diagnostics.TraceEventType,System.Int32,System.String,System.Object[],System.Object,System.Object[])
additional_notes.overrides: *content
---

<p>Implementations of this method should return `true` if the event specified by the passed parameters should be traced. Otherwise the method should return `false`. For example, a filter that allows only error events to pass through to the listener should inspect the <code>eventType</code> parameter and return `true` if the trace event type level is set to <xref href="System.Diagnostics.TraceEventType.Error"></xref> or greater; otherwise, it should return `false`.  
  
 Implementations of the method should be prepared to handle `null` in the following parameters: <code>args</code>, <code>data1</code>, <code>data</code>, <code>formatOrMessage</code>, and <code>cache</code>. If the parameter value is `null`, the parameter is not part of the event. For example, if the <code>args</code> parameter is `null`, it means that the event does not have any arguments. If the <code>data</code> parameter is `null`, then there are either one or no data objects. If there is one data object, it will be found in the <code>data1</code> parameter. The reason for the distinction between a single data object and an array of data objects is for performance. There is no reason to create an object array if only one object is traced, as is normally the case. If the <code>data</code> parameter is not `null`, the <code>data1</code> parameter must also not be `null`.  
  
 It is guaranteed that the <code>source</code> parameter is not `null` and not an empty string ("").  
  
 Implementations of the method can optionally throw the following exceptions:  
  
-   <xref href="System.ArgumentNullException"></xref> if <code>source</code> is `null`.  
  
-   <xref href="System.ArgumentException"></xref> if <code>eventType</code> is not one of the <xref href="System.Diagnostics.TraceEventType"></xref> values.  
  
-   Exceptions unrelated to the implementation of the method. For example, a <xref href="System.Threading.ThreadAbortException"></xref>.</p>


