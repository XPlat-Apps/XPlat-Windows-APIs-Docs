# TypedEventHandler delegate

> Namespace: XPlat.Foundation

Represents a method that handles general events.

```csharp
public delegate void TypedEventHandler<in TSender, in TResult>(TSender sender, TResult args);
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 