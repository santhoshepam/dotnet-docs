---
uid: System.ServiceModel.Dispatcher.IMessageFilterTable`1
thread_safety: *content
---

Filter tables are thread-safe with respect to matching operations, but are not thread-safe with respect to modification. Threads that access a filter table should be synchronized by the <xref href="System.Threading.ReaderWriterLock"></xref> or similar locking semantic. This lock allows multiple reads of a filter table (for example, a match operation) to run simultaneously, but in order to write to a filter table (for example, adding a filter), a thread must wait for an exclusive lock.  
  
 All compilation is done when filters are added to the table. If you create a filter table in advance, and never edit it, locking is not necessary during a match.


