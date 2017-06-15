---
uid: System.Threading.SpinWait
thread_safety: *content
---

While <xref href="System.Threading.SpinWait"></xref> is designed to be used in concurrent applications, it is not designed to be used from multiple threads concurrently. <xref href="System.Threading.SpinWait"></xref> members are not thread-safe. If multiple threads must spin, each should use its own instance of <xref href="System.Threading.SpinWait"></xref>.


