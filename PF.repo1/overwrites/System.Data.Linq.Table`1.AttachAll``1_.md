---
summary: Attaches all entities of a collection to the <xref href="System.Data.Linq.DataContext"></xref> in either a modified or unmodified state.
remarks: "If attaching as modified, the entity must either declare a version member or must not participate in update conflict checking.  \n  \n When a new entity is attached, deferred loaders for any child collections (for example, `EntitySet` collections of entities from associated tables) are initialized. When <xref:System.Data.Linq.DataContext.SubmitChanges%2A> is called, members of the child collections are put into an `Unmodified` state. To update members of a child collection, you must explicitly call `Attach` and specify that entity.  \n  \n For more information, see [Data Retrieval and CUD Operations in N-Tier Applications (LINQ to SQL)](~/docs/framework/data/adonet/sql/linq/data-retrieval-and-cud-operations-in-n-tier-applications.md)."
uid: System.Data.Linq.Table`1.AttachAll``1*
---
