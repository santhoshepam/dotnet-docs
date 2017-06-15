---
uid: System.Web.Hosting.ISuspendibleRegisteredObject
thread_safety: *content
---

Instance members of this type are not guaranteed to be thread safe. You can call the <xref href="System.Web.Hosting.ISuspendibleRegisteredObject.Suspend"></xref> method at any time, including during a call to another method on this same object, during calls to other objects' <xref href="System.Web.Hosting.ISuspendibleRegisteredObject.Suspend"></xref> methods, or even during a call to this object's <xref href="System.Web.Hosting.ISuspendibleRegisteredObject.Suspend"></xref> method. Because the execution of these methods is multithreaded, there is an interval in which the <xref href="System.Web.Hosting.ISuspendibleRegisteredObject.Suspend"></xref> method can be called even after a call to the <xref href="System.Web.Hosting.HostingEnvironment.UnregisterObject(System.Web.Hosting.IRegisteredObject)"></xref> method has completed.


