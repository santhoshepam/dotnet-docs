---
uid: System.DateTime
remarks: *content
---

The @System.DateTime value type represents dates and times with values ranging from 00:00:00 (midnight), January 1, 0001 Anno Domini (Common Era) through 11:59:59 P.M., December 31, 9999 A.D. (C.E.) in the Gregorian calendar.

Time values are measured in 100-nanosecond units called ticks, and a particular date is the number of ticks since 12:00 midnight, January 1, 0001 A.D. (C.E.) in the @System.Globalization.GregorianCalendar calendar (excluding ticks that would be added by leap seconds). For example, a ticks value of 31241376000000000L represents the date, Friday, January 01, 0100 12:00:00 midnight. A @System.DateTime value is always expressed in the context of an explicit or default calendar.

> [!NOTE]
> If you are working with a ticks value that you want to convert to some other time interval, such as minutes or seconds, you should use the @System.TimeSpan.TicksPerDay, @System.TimeSpan.TicksPerHour, @System.TimeSpan.TicksPerMinute, @System.TimeSpan.TicksPerSecond, or @System.TimeSpan.TicksPerMillisecond constant to perform the conversion. For example, to add the number of seconds represented by a specified number of ticks to the @System.DateTime.Second component of a @System.DateTime value, you can use the expression `dateValue.Second + nTicks/Timespan.TicksPerSecond`

In this section:

- [Instantiating a DateTime object](#instantiating_datetime)
- [DateTime values and their string representations](#instantiating_datetime)
- [Converting strings to DateTime values](#instantiating_datetime)
- [Version considerations](#instantiating_datetime)
- [DateTime values](#instantiating_datetime) 
- [DateTime operations](#instantiating_datetime)
- [DateTime resolution](#instantiating_datetime)
- [DateTime vs. TimeSpan](#instantiating_datetime)
- [DateTime values and calendars](#instantiating_datetime)
- [Persisting DateTime values](#instantiating_datetime)
- [COM interop considerations](#instantiating_datetime)

# <href a="instantiating_datetime"/>Instantiating a DateTime object #

You can create a new @System.DateTime value in any of the following ways:

- By calling any of the overloads of the @System.DateTime constructor that allow you to specify specific elements of the date and time value (such as the year, month, and day, or the number of ticks). The following code illustrates a call to one of the @System.DateTime constructors to create a date with a specific year, month, day, hour, minute, and second.

[!code-csharp[Instantating](../samples/snippets/csharp/instantiation1.cs#L17)]
[!code-vb[Instantiating](../samples/snippets/vb/instantiation1.vb#L17)]

- By using any compiler-specific syntax for declaring date and time values. For example, the following Visual Basic statement initializes a new @System.DateTime value.

[!code-vb[Instantiating](../samples/snippets/vb/instantiation1.vb#L23)]


                <maml:listItem>
                  <maml:para>By assigning the @System.DateTime</maml:codeEntityReference> object a date and time value returned by a property or method. The following example assigns the current date and time, the current Coordinated Universal Time (UTC) date and time, and the current date to three new @System.DateTime</maml:codeEntityReference> variables. </maml:para>
                  <maml:codeReference>System.DateTime.Instantiation#3</maml:codeReference>
                </maml:listItem>
                <maml:listItem>
                  <maml:para>By parsing the string representation of a date and time value. The <maml:codeEntityReference autoUpgrade="true">Overload:System.DateTime.Parse</maml:codeEntityReference>, <maml:codeEntityReference autoUpgrade="true">Overload:System.DateTime.ParseExact</maml:codeEntityReference>, <maml:codeEntityReference autoUpgrade="true">Overload:System.DateTime.TryParse</maml:codeEntityReference>, and <maml:codeEntityReference autoUpgrade="true">Overload:System.DateTime.TryParseExact</maml:codeEntityReference> methods all convert a string to its equivalent date and time value. The following example uses the <maml:codeEntityReference autoUpgrade="true">M:System.DateTime.Parse(System.String,System.IFormatProvider)</maml:codeEntityReference> method to parse a string and convert it to a @System.DateTime</maml:codeEntityReference> value. </maml:para>
                  <maml:codeReference>System.DateTime.Instantiation#4</maml:codeReference>
                  <maml:para>
                    <?Comment rcp: This section addresses several customer complaints that there is no illustration of how to createDateTimevalues. 2014-05-09T08:37:00Z  Id='2?>Note that the <maml:codeEntityReference autoUpgrade="true">Overload:System.DateTime.TryParse</maml:codeEntityReference> and <maml:codeEntityReference autoUpgrade="true">Overload:System.DateTime.TryParseExact</maml:codeEntityReference> methods indicate whether a particular string contains a valid representation of a @System.DateTime</maml:codeEntityReference> value in addition to performing the conversion. </maml:para>
                </maml:listItem>
                <maml:listItem>
                  <maml:para>By calling the @System.DateTime</maml:codeEntityReference> structure's implicit default constructor. (For details on the implicit default constructor of a value type, see <maml:link xlink:href="471eb994-2958-49d5-a6be-19b4313f80a3">Value Types (C# Reference)</maml:link>.) An approximate equivalent, for compilers that support it, is declaring a @System.DateTime</maml:codeEntityReference>  value without explicitly assigning a date and time to it. The following example illustrates a call to the @System.DateTime</maml:codeEntityReference> implicit default constructor in C# and Visual Basic, as well as a @System.DateTime</maml:codeEntityReference> variable declaration with no assignment in Visual Basic.</maml:para>
                  <maml:codeReference>System.DateTime.Instantiation#5</maml:codeReference>
                </maml:listItem>
              </maml:list>
            </maml:content>
          </maml:section>

