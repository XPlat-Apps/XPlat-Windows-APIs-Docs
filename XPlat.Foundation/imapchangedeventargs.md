# IMapChangedEventArgs interface

> Namespace: XPlat.Foundation.Collections

Provides data for the changed event of a map collection.

```csharp
public interface IMapChangedEventArgs<K>
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### CollectionChange

Gets the type of change that occurred in the map.

```csharp
CollectionChange CollectionChange { get; }
```

### Key

Gets the key of the item that changed.

```csharp
K Key { get; }
```

## Related information

### References

[IMapChangedEventArgs<K> - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.foundation.collections.imapchangedeventargs_k_)