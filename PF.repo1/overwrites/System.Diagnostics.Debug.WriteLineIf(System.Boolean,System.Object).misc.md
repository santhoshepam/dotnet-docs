---
uid: System.Diagnostics.Debug.WriteLineIf(System.Boolean,System.Object)
additional_notes.overrides: *content
---

<p>You can minimize the performance penalty of instrumenting your application by using `If...Then` statements instead of using <xref href="System.Diagnostics.Debug.WriteLineIf(System.Boolean,System.String)"></xref> statements. The following two code examples send the same debugging message. However, the first example is much faster when tracing is off, because if <code>mySwitch.TraceError</code> evaluates to `false`, you do not call <xref href="System.Diagnostics.Debug.WriteLine(System.String)"></xref>. The second example always calls <xref href="System.Diagnostics.Debug.WriteLineIf(System.Boolean,System.String)"></xref>, even when <code>mySwitch.TraceError</code> is `false` and no tracing output is produced. This can result in unnecessary execution of arbitrarily complex code.  
  
 First example:  
  
```  
if(mySwitch.TraceError)   
    Debug.WriteLine("aNumber = " + aNumber + " out of range");  
```  
  
 Second example:  
  
```  
Debug.WriteLineIf(mySwitch.TraceError, "aNumber = " + aNumber + " out of range");  
```</p>


