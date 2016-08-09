---
uid: System.Net.Http.HttpClient
remarks: >
    The @System.Net.Http.HttpClient class instance acts as a session to send HTTP requests. 
An @System.Net.Http.HttpClient instance is a collection of settings applied to all requests executed by that instance. 
In addition, every @System.Net.Http.HttpClient instance uses its own connection pool, isolating its requests from requests executed by other @System.Net.Http.HttpClient instances.
    The @System.Net.Http.HttpClient also acts as a base class for more specific HTTP clients. 
An example would be a FacebookHttpClient providing additional methods specific to a Facebook web service (a GetFriends method, for instance).
    By default, @System.Net.HttpWebRequest will be used to send requests to the server. 
This behavior can be modified by specifying a different channel in one of the constructor overloads taking a @System.Net.Http.HttpMessageHandler instance as parameter. 
If features like authentication or caching are required, @System.Net.Http.WebRequestHandler can be used to configure settings and the instance can be passed to the constructor. 
The returned handler can be passed to one of the constructor overloads taking a @System.Net.Http.HttpMessageHandler parameter.
    If an app using @System.Net.Http.HttpClient and related classes in the @System.Net.Http namespace intends to download large amounts of data (50 megabytes or more), then the app should stream those downloads and not use the default buffering. 
If the default buffering is used the client memory usage will get very large, potentially resulting in substantially reduced performance.
---
uid: System.Net.Http.HttpClient.CancelPendingRequests
remarks: After calling this method, the @System.Net.Http.HttpClient instance can still be used to execute additional requests.
---