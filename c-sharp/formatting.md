# C# / Formatting strings and numbers

### Formatting a Decimal value as currency

```C#
var value = 1234.50m;
var formatted = value.ToString("C", CultureInfo.GetCultureInfo("sv-SE"));

// formatted is "1 234,50 kr"
// CultureInfo.CurrentCulture can be used instead of GetCultureInfo
```

More info: [Currency format specifier](https://docs.microsoft.com/en-us/dotnet/standard/base-types/standard-numeric-format-strings#CFormatString)
