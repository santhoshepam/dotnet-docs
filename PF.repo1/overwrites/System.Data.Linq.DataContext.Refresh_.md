---
summary: Refreshes object state by using data in the database.
remarks: "This method is useful after an optimistic concurrency error to bring items into a state for another attempt. It updates the state of the primitive fields and properties on the objects.  \n  \n> [!NOTE]\n>  If an object is on the *many* side of a one-to-many relationship, the foreign key on the object will be set and the object pointer for the other side of the relationship will be set to the new value."
uid: System.Data.Linq.DataContext.Refresh*
---
