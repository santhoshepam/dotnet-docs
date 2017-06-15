---
uid: System.ConsoleCancelEventArgs.Cancel
additional_notes.usage: *content
---

<p>In the [!INCLUDE[net_v35_short](~/includes/net-v35-short-md.md)] and [!INCLUDE[net_v40_short](~/includes/net-v40-short-md.md)], attempting to set the <xref href="System.ConsoleCancelEventArgs.Cancel"></xref> property to `true` if the <xref href="System.Console.CancelKeyPress"></xref> event was invoked by the user pressing Ctrl+Break threw an <xref href="System.InvalidOperationException"></xref> exception. In the [!INCLUDE[net_v45](~/includes/net-v45-md.md)], you can set the <xref href="System.ConsoleCancelEventArgs.Cancel"></xref> property to `true` after the user presses Ctrl+Break and cancel the termination of the application.</p>


