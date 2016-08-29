---
uid: System.Sample.Random()
remarks: *content
---
To produce a different random distribution or a implement a different random number generation algorithm, drive a class from the @System.Random class and override the @System.Random.Sample method.

> [!Note:]
> The @System.Random.Sample method is `protected`, which means that it is accessible only within the @System.Random class and its derived classes. To generate a random number between 0 and 1 from a @System.Random instance, call the @Random.NextDouble method.
