# C# / Collections

### Extend the size of an array

```C#
// Create an array
int[] myArray = new int[3];     // myArray.Length is 3

// Extend the size of the array and copy old elements over
Array.Resize(ref myArray, 5);   // myArray.Length is now 5
```

More info: [Array.Resize<T>(T[], Int32) Method](https://docs.microsoft.com/en-us/dotnet/api/system.array.resize?view=net-6.0)
