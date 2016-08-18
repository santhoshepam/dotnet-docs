---
uid: System.Numerics.BigInteger
remarks: *content
---
The @System.Numerics.BigInteger type is an immutable type that represents an arbitrarily large integer whose value in theory has no upper or lower bounds. 
The members of the @System.Numerics.BigInteger type closely parallel those of other integral types (the @System.Byte, @System.Int16, @System.Int32, @System.Int64, @System.SByte, @System.UInt16, @System.UInt32, and @System.UInt64 types). 
This type differs from the other integral types in the .NET Framework, which have a range indicated by their `MinValue` and `MaxValue` properties.

> [!NOTE]
> Because the @System.Numerics.BigInteger type is immutable (see [Mutability and the BigInteger Structure](https://msdn.microsoft.com/en-us/library/system.numerics.biginteger.aspx#mutability)) and because it has no upper or lower bounds, 
> an @System.OutOfMemoryException can be thrown for any operation that causes a @System.Numerics.BigInteger value to grow too large.

##Instantiating a BigInteger object
You can instantiate a @System.Numerics.BigInteger object in several ways:

- You can use the `new` keyword and provide any integral or floating-point value as a parameter to the @System.Numerics.BigInteger constructor. 
(Floating-point values are truncated before they are assigned to the @System.Numerics.BigInteger .) 
The following example illustrates how to use the `new` keyword to instantiate @System.Numerics.BigInteger values.

```csharp
BigInteger bigIntFromDouble = new BigInteger(179032.6541);
Console.WriteLine(bigIntFromDouble);
BigInteger bigIntFromInt64 = new BigInteger(934157136952);
Console.WriteLine(bigIntFromInt64);
// The example displays the following output:
//   179032
//   934157136952	
```

- You can declare a @System.Numerics.BigInteger variable and assign it a value just as you would any numeric type, as long as that value is an integral type. 
The following example uses assignment to create a @System.Numerics.BigInteger value from an @System.Int64.

```csharp
long longValue = 6315489358112;      
BigInteger assignedFromLong = longValue;
Console.WriteLine(assignedFromLong);
// The example displays the following output:
//   6315489358112
```

- You can assign a decimal or floating-point value to a @System.Numerics.BigInteger object if you cast the value or convert it first. 
The following example explicitly casts (in C#) or converts (in Visual Basic) a @System.Double and a @System.Decimal value to a @System.Numerics.BigInteger.

```csharp
BigInteger assignedFromDouble = (BigInteger) 179032.6541;
Console.WriteLine(assignedFromDouble);   
BigInteger assignedFromDecimal = (BigInteger) 64312.65m;      
Console.WriteLine(assignedFromDecimal);
// The example displays the following output:
//   179032
//   64312   
```