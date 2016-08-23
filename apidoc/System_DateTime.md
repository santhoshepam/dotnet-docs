---
uid: System.DateTime
remarks: *content
---

The @System.DateTime value type represents dates and times with values ranging from 00:00:00 (midnight), January 1, 0001 Anno Domini (Common Era) through 11:59:59 P.M., December 31, 9999 A.D. (C.E.) in the Gregorian calendar.

Time values are measured in 100-nanosecond units called ticks, and a particular date is the number of ticks since 12:00 midnight, January 1, 0001 A.D. (C.E.) in the @System.Globalization.GregorianCalendar calendar (excluding ticks that would be added by leap seconds). For example, a ticks value of 31241376000000000L represents the date, Friday, January 01, 0100 12:00:00 midnight. A @System.DateTime value is always expressed in the context of an explicit or default calendar.

> [!NOTE]
> If you are working with a ticks value that you want to convert to some other time interval, such as minutes or seconds, you should use the @System.TimeSpan.TicksPerDay, @System.TimeSpan.TicksPerHour, @System.TimeSpan.TicksPerMinute, @System.TimeSpan.TicksPerSecond, or @System.TimeSpan.TicksPerMillisecond constant to perform the conversion. For example, to add the number of seconds represented by a specified number of ticks to the @System.DateTime.Second component of a @System.DateTime value, you can use the expression `dateValue.Second + nTicks/Timespan.TicksPerSecond`

In this section:

- [Instantiating a DateTime object](#Instantiation)
- [DateTime values and their string representations](#Strings)
- [Converting strings to DateTime values](#Instantiation)
- [Version considerations](#Instantiation)
- [DateTime values](#Instantiation) 
- [DateTime operations](#Instantiation)
- [DateTime resolution](#Instantiation)
- [DateTime vs. TimeSpan](#Instantiation)
- [DateTime values and calendars](#Instantiation)
- [Persisting DateTime values](#Instantiation)
- [COM interop considerations](#Instantiation)

<a name="Instantiation"></a>
## Instantiating a DateTime object ##

You can create a new @System.DateTime value in any of the following ways:

- By calling any of the overloads of the @System.DateTime constructor that allow you to specify specific elements of the date and time value (such as the year, month, and day, or the number of ticks). The following code illustrates a call to one of the @System.DateTime constructors to create a date with a specific year, month, day, hour, minute, and second.

  [!code-csharp[Instantating](../samples/snippets/csharp/System.DateTime/instantiation1.cs#L17-L17)]
  [!code-vb[InstantiatingVB](../samples/snippets/vb/System.DateTime/instantiation1.vb#L17-L17)]

- By using any compiler-specific syntax for declaring date and time values. For example, the following Visual Basic statement initializes a new @System.DateTime value.

  [!code-vb[InstantiatingVB](../samples/snippets/vb/System.DateTime/instantiation1.vb#L23-L23)]

- By assigning the @System.DateTime object a date and time value returned by a property or method. The following example assigns the current date and time, the current Coordinated Universal Time (UTC) date and time, and the current date to three new @System.DateTime variables.

  [!code-csharp[Instantating](../samples/snippets/csharp/System.DateTime/instantiation1.cs#L24-L26)]
  [!code-visualbasic[InstantiatingVB](../samples/snippets/vb/System.DateTime/instantiation1.vb#L29-L31)]

- By parsing the string representation of a date and time value. Overloads of the @System.DateTime.Parse(System.String), @System.DateTime.ParseExact(System.String,System.String,System.IFormatProvider), @System.DateTime.TryParse(System.String,System.DateTime), and @System.DateTime.TryParseExact(System.String,System.String,System.IFormatProvider,System.Globalization.DateTimeStyles,System.DateTime) methods all convert a string to its equivalent date and time value. The following example uses the @System.DateTime.Parse(System.String,System.IFormatProvider) method to parse a string and convert it to a @System.DateTime value.

  [!code-csharp[Instantating](../samples/snippets/csharp/System.DateTime/instantiation1.cs#L33-L35)]
  [!code-vb[InstantiatingVB](../samples/snippets/vb/System.DateTime/instantiation1.vb#L37-L39)]

  Note that the @System.DateTime.TryParse and @System.DateTime.TryParseExact methods indicate whether a particular string contains a valid representation of a @System.DateTime value in addition to performing the conversion.

- By calling the @System.DateTime structure's implicit default constructor. (For details on the implicit default constructor of a value type, see [Value Types (C# Reference)](https://msdn.microsoft.com/library/s1ax56ch.aspx).) An approximate equivalent, for compilers that support it, is declaring a @System.DateTime value without explicitly assigning a date and time to it. The following example illustrates a call to the @System.DateTime implicit default constructor in C# and Visual Basic, as well as a @System.DateTime variable declaration with no assignment in Visual Basic.

  [!code-csharp[Instantating](../samples/snippets/csharp/System.DateTime/instantiation1.cs#L42-L46)]
  [!code-vb[InstantiatingVB](../samples/snippets/vb/System.DateTime/instantiation1.vb#L46-L56)]

<a name="Strings"></a>
## DateTime values and their string representations ##

Internally, all @System.DateTime values are represented as the number of ticks (the number of 100-nanosecond intervals) that have elapsed since 12:00:00 midnight, January 1, 0001. The actual @System.DateTime value is independent of the way in which that value appears when displayed in a user interface element or when written to a file. The appearance of a @System.DateTime value is the result of a formatting operation. Formatting is the process of converting a value to its string representation.

Because the appearance of date and time values is dependent on such factors as culture, international standards, application requirements, and personal preference, the @System.DateTime structure offers a great deal of flexibility in formatting date and time values through the overloads of its @System.DateTime.ToString method. The default @System.DateTime.ToString method returns the string representation of a date and time value using the current culture's short date and long time pattern. The following example uses the default @System.DateTime.ToString method to display the date and time using the short date and long time pattern for the en-US culture, the current culture on the computer on which the example was run.

[!code-csharp[Formatting](../samples/snippets/csharp/System.DateTime/formatting1.cs)]
[!code-vb[FormattingVB](../samples/snippets/vb/System.DateTime/formatting1.vb)]

