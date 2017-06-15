---
summary: Initializes a new instance of the <xref href="System.Net.Http.HttpClient"></xref> class.
remarks: "<xref:System.Net.Http.HttpClient> is intended to be instantiated once and re-used throughout the life of an application. Instantiating an HttpClient class for every request will exhaust the number of sockets available under heavy loads. This will result in SocketException errors. Below is an example using HttpClient correctly.  \n  \n```csharp  \npublic class GoodController : ApiController  \n{  \n    // OK  \n    private static readonly HttpClient HttpClient;  \n  \n    static GoodController()  \n    {  \n        HttpClient = new HttpClient();  \n    }  \n}  \n  \n```"
uid: System.Net.Http.HttpClient.#ctor*
---
