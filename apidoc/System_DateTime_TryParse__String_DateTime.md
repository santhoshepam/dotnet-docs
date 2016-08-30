---
uid: System.DateTime.TryParse(System.String,System.DateTime@)
remarks: *content
---
The @System.DateTime.TryParse(System.String,System.DateTime@) method is similar to the @System.DateTime.Parse(System.String) method, except that the @System.DateTime.TryParse(System.String,System.DateTime@) method does not throw an exception if the conversion fails.

The string `s` is parsed using formatting information in the current @System.Globalization.DateTimeFormatInfo object, which is supplied implicitly by the current thread culture.

This method tries to ignore unrecognized data, if possible, and fills in missing month, day, and year information with the current date. If `s` contains only a date and no time, this method assumes the time is 12:00 midnight. If `s` includes a date component with a two-digit year, it is converted to a year in the current culture's current calendar based on the value of the @System.Globalization.Calendar.TwoDigitYearMax property. Any leading, inner, or trailing white space character in `s` is ignored. The date and time can be bracketed with a pair of leading and trailing NUMBER SIGN characters ('#', U+0023), and can be trailed with one or more NULL characters (U+0000).

Because the @System.DateTime.TryParse(System.String,System.DateTime@) method tries to parse the string representation of a date and time using the formatting rules of the current culture, trying to parse a particular string across different cultures can either fail or return different results. If a specific date and time format will be parsed across different locales, use the @System.DateTime.TryParse(System.String,System.IFormatProvider,System.Globalization.DateTimeStyles,System.DateTime@) method or one of the overloads of the `System.DateTime.TryParseExact` method and provide a format specifier.

If `s` is the string representation of a leap day in a leap year in the current calendar, the method parses `s` successfully. If `s` is the string representation of a leap day in a non-leap year in the current culture's current calendar, the parse operation fails and the method returns `false`.

If `s` contains no time zone information, `result` contains a @System.DateTime value whose @System.DateTime.Kind property is @System.DateTimeKind.Unspecified when the method returns. If the string to be parsed contains time zone information, `result` contains a @System.DateTime value whose @System.DateTime.Kind property is @System.DateTimeKind.Local when the method returns.

## Notes for Callers ##

In the .NET Framework, formatting is influenced by properties of the current @System.Globalization.DateTimeFormatInfo object, which by default are derived from the *Regional and Language Options* item in Control Panel. The `System.DateTime.TryParse` method can unexpectedly fail and return `false` if the current @System.Globalization.DateTimeFormatInfo.DateSeparator and @System.Globalization.DateTimeFormatInfo.TimeSeparator properties are set to the same value.

The @System.Globalization.DateTimeFormatInfo.DateSeparator and @System.Globalization.DateTimeFormatInfo.TimeSeparator properties are not available in .NET Core.
