---
uid: System.Random.Sample()
remarks: *content
---

To produce a different random distribution or a implement a different random number generation algorithm, drive a class from the @System.Random class and override the @System.Random.Sample method.

> [!Note:]
> The @System.Random.Sample method is `protected`, which means that it is accessible only within the @System.Random class and its derived classes. To generate a random number between 0 and 1 from a @System.Random instance, call the @Random.NextDouble method.


---
uid: System.Random.Sample
remarks: *content
---

To produce a different random distribution or a implement a different random number generation algorithm, drive a class from the @System.Random class and override the @System.Random.Sample method.

> [!Note:]
> The @System.Random.Sample method is `protected`, which means that it is accessible only within the @System.Random class and its derived classes. To generate a random number between 0 and 1 from a @System.Random instance, call the @Random.NextDouble method.

### Notes to Inheritors ###

Starting with the .NET Framework version 2.0, if you derive a class from @System.Random and override the @System.Random.Sample method, the distribution provided by the derived class implementation of the @System.Random.Sample method is not used in calls to the base class implementation of the following methods:

- The Random.NextBytes(Byte[]) method.

- The Random.Next() method.

- The Random.Next(Int32, Int32) method, if (maxValue - minValue) is greater than Int32.MaxValue.

Instead, the uniform distribution provided by the base @System.Random class is used. This behavior improves the overall performance of the Random class. To modify this behavior to call the implementation of the @System.Random.Sample method in the derived class, you must also override the behavior of these three members. The example provides an illustration.

