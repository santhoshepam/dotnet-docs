---
uid: System.IAsyncResult.AsyncWaitHandle
additional_notes.overrides: *content
---

<p>The object that implements <xref href="System.IAsyncResult"></xref> does not need to create the <xref href="System.Threading.WaitHandle"></xref> until the <xref href="System.IAsyncResult.AsyncWaitHandle"></xref> property is read. It is the choice of the <xref href="System.IAsyncResult"></xref> implementer. However, if the implementer creates <xref href="System.IAsyncResult.AsyncWaitHandle"></xref>, it is the responsibility of the implementer to signal the <xref href="System.Threading.WaitHandle"></xref> that will terminate the wait at the appropriate time. For example, <xref href="System.Runtime.Remoting.Messaging.AsyncResult"></xref> terminates the wait on behalf of the caller when an asynchronously invoked method returns. Once created, <xref href="System.IAsyncResult.AsyncWaitHandle"></xref> should be kept alive until the user calls the method that concludes the asynchronous operation. At that time the object behind <xref href="System.IAsyncResult.AsyncWaitHandle"></xref> can be discarded.</p>


---
uid: System.IAsyncResult.AsyncWaitHandle
additional_notes.usage: *content
---

<p>Clients that wait for the operation to complete (as opposed to polling) use this property to obtain a synchronization object to wait on.  
  
 <block subset="none" type="note"><p>  
 When you use the `BeginInvoke` method of a delegate to call a method asynchronously and obtain a wait handle from the resulting <xref href="System.IAsyncResult"></xref>, we recommend that you close the wait handle as soon as you are finished using it, by calling the <xref href="System.Threading.WaitHandle.Close"></xref> method. If you simply release all references to the wait handle, system resources are freed when garbage collection reclaims the wait handle, but garbage collection works more efficiently when disposable objects are explicitly closed or disposed. For more information, see the <xref href="System.Runtime.Remoting.Messaging.AsyncResult.AsyncWaitHandle"></xref> property.  
  
</p></block></p>


