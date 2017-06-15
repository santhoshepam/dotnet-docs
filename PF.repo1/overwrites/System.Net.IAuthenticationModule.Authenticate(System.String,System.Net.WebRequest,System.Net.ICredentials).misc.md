---
uid: System.Net.IAuthenticationModule.Authenticate(System.String,System.Net.WebRequest,System.Net.ICredentials)
additional_notes.overrides: *content
---

<p>The <xref href="System.Net.AuthenticationManager"></xref> calls the <xref href="System.Net.IAuthenticationModule.Authenticate(System.String,System.Net.WebRequest,System.Net.ICredentials)"></xref> method on registered authentication modules to determine which module handles the challenge. If the authentication module cannot handle the challenge, the <xref href="System.Net.IAuthenticationModule.Authenticate(System.String,System.Net.WebRequest,System.Net.ICredentials)"></xref> method must return `null`. If the authentication module encounters an error while conducting the authentication process, <xref href="System.Net.IAuthenticationModule.Authenticate(System.String,System.Net.WebRequest,System.Net.ICredentials)"></xref> must throw an exception.</p>


