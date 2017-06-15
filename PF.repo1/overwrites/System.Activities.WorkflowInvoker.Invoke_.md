---
summary: Invokes a workflow synchronously and returns a dictionary of the root activity’s <xref href="System.Activities.OutArgument"></xref> and <xref href="System.Activities.InOutArgument"></xref> values keyed by argument name that represent the outputs of the workflow.
remarks: This method blocks until the workflow has completed, including idle time. All workflow execution is guaranteed to execute on the invoking thread. To configure a time-out interval in which the workflow must complete, use one of the <xref:System.Activities.WorkflowInvoker.Invoke%2A> overloads that take a <xref:System.TimeSpan>.
uid: System.Activities.WorkflowInvoker.Invoke*
---
