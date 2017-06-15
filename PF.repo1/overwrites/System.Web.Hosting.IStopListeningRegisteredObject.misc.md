---
uid: System.Web.Hosting.IStopListeningRegisteredObject
thread_safety: *content
---

Instance members of this type are not guaranteed to be thread safe. The <xref href="System.Web.Hosting.IStopListeningRegisteredObject.StopListening"></xref> method can be called at any time, including while a call to another method (such as <xref href="System.Web.Hosting.IRegisteredObject.Stop(System.Boolean)"></xref>) on this same object is executing or while calls to other objects' <xref href="System.Web.Hosting.IStopListeningRegisteredObject.StopListening"></xref> methods are executing. Because the execution of these methods is multithreaded, there is an interval in which the <xref href="System.Web.Hosting.IStopListeningRegisteredObject.StopListening"></xref> method might be called even after a call to <xref href="System.Web.Hosting.HostingEnvironment.UnregisterObject(System.Web.Hosting.IRegisteredObject)"></xref> has completed.


