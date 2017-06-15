---
summary: Computes the set of modified objects to be inserted, updated, or deleted, and executes the appropriate commands to implement the changes to the database.
remarks: "If override methods are present for insert, update, or delete, <xref:System.Data.Linq.DataContext.SubmitChanges%2A> executes these methods instead of the default [!INCLUDE[vbtecdlinq](~/includes/vbtecdlinq-md.md)] commands.  \n  \n <xref:System.Data.Linq.DataContext.SubmitChanges%2A> starts a transaction and will roll back if an exception occurs while <xref:System.Data.Linq.DataContext.SubmitChanges%2A> is executing. However, this does not roll back the changes in memory or tracked by the <xref:System.Data.Linq.DataContext>; those changes will need to be rolled back manually. You can start with a new instance of the <xref:System.Data.Linq.DataContext> if the changes in memory are to be discarded."
uid: System.Data.Linq.DataContext.SubmitChanges*
---
