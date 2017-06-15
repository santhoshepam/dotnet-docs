---
uid: System.Runtime.InteropServices.SafeHandle
additional_notes.overrides: *content
---

<p>To create a class derived from <xref href="System.Runtime.InteropServices.SafeHandle"></xref>, you must know how to create and free an operating system handle. This process is different for different handle types because some use the [CloseHandle](https://msdn.microsoft.com/library/windows/desktop/ms724211.aspx) function, while others use more specific functions such as [UnmapViewOfFile](https://msdn.microsoft.com/library/windows/desktop/aa366882.aspx) or [FindClose](https://msdn.microsoft.com/library/windows/desktop/aa364413.aspx). For this reason, you must create a derived class of <xref href="System.Runtime.InteropServices.SafeHandle"></xref> for each operating system handle type that you want to wrap in a safe handle.  
  
 When you inherit from <xref href="System.Runtime.InteropServices.SafeHandle"></xref>, you must override the following members: <xref href="System.Runtime.InteropServices.SafeHandle.IsInvalid"></xref> and <xref href="System.Runtime.InteropServices.SafeHandle.ReleaseHandle"></xref>.  
  
 You should also provide a default constructor that calls the base constructor with a value that represent an invalid handle value, and a <xref href="System.Boolean"></xref> value indicating whether the native handle is owned by the <xref href="System.Runtime.InteropServices.SafeHandle"></xref> and consequently should be freed when that <xref href="System.Runtime.InteropServices.SafeHandle"></xref> has been disposed.</p>


