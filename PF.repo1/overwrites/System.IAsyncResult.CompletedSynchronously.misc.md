---
uid: System.IAsyncResult.CompletedSynchronously
additional_notes.overrides: *content
---

<p>Most implementers of the <xref href="System.IAsyncResult"></xref> interface will not use this property and should return `false`. Beginning with the [!INCLUDE[net_v45](~/includes/net-v45-md.md)], a task that is created with the <xref href="System.Threading.Tasks.TaskFactory.FromAsync(System.IAsyncResult,System.Action{System.IAsyncResult},System.Threading.Tasks.TaskCreationOptions)"></xref> method will not complete if this property is not implemented correctly. See [Application Compatibility in 4.5](~/docs/framework/migration-guide/application-compatibility-in-the-net-framework-4-5.md).</p>


---
uid: System.IAsyncResult.CompletedSynchronously
additional_notes.usage: *content
---

<p>Use this property to determine if the asynchronous operation completed synchronously. For example, this property can return `true` for an asynchronous I/O operation if the I/O request was small.</p>


