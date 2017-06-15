---
summary: Persists a workflow instance to an instance store.
remarks: If the workflow instance was previously loaded from persistence, then the same <xref:System.Runtime.DurableInstancing.InstanceStore> used to load the workflow is used for persistence. If the workflow was created and has not yet been persisted, then an <xref:System.Activities.WorkflowApplication.InstanceStore%2A> must be configured before calling this method or else an <xref:System.InvalidOperationException> is thrown when this method is called.
uid: System.Activities.WorkflowApplication.Persist*
---
