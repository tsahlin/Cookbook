# C# / Operators

### Indexer

```C#
public string this[int key]
{
    get => GetValue(key);
    set => SetValue(key, value);
}
```

More info: [Using indexers](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/indexers/using-indexers)
