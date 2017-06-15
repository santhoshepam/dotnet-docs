---
summary: Displays a common dialog.
remarks: "<xref:Microsoft.Win32.CommonDialog.ShowDialog%2A> performs initialization tasks for all common dialogs before calling <xref:Microsoft.Win32.CommonDialog.RunDialog%2A>. Since <xref:Microsoft.Win32.CommonDialog.RunDialog%2A> requires an owner window, <xref:Microsoft.Win32.CommonDialog.ShowDialog%2A> attempts to assign one in the following order of precedence:  \n  \n-   The current application's *active window*.  \n  \n-   The current application's *parking window*.  \n  \n-   An internally generated hidden window."
uid: Microsoft.Win32.CommonDialog.ShowDialog*
---
