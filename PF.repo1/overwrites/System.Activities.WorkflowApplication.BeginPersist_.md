---
summary: Persists a workflow instance to an instance store asynchronously using the <xref href="System.IAsyncResult"></xref> asynchronous design pattern.
remarks: "[!INCLUDE[crdefault](~/includes/crdefault-md.md)] [Asynchronous Programming Overview](http://go.microsoft.com/fwlink/?LinkId=141764).  \n  \n If the workflow instance was previously loaded from persistence, then the same <xref:System.Runtime.DurableInstancing.InstanceStore> used to load the workflow is used for persistence. If the workflow was created and has not yet been persisted, then an <xref:System.Activities.WorkflowApplication.InstanceStore%2A> must be configured before calling this method or else an <xref:System.InvalidOperationException> is thrown when this method is called."
uid: System.Activities.WorkflowApplication.BeginPersist*
---
