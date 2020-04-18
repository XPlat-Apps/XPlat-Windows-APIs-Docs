# MapLocationDesiredAccuracy enum

> Namespace: XPlat.Services.Maps

Indicates the desired accuracy to use when converting latitude and longitude coordinates to a physical location like a city or address.

```csharp
public enum MapLocationDesiredAccuracy
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Fields

| Enum Value | Int Value | Description |
| --- | --- | --- |
| High | 0 | Leverage the underlying REST API call to get richer and more accurate results. |
| Low | 1 | Leverage the maps disk cache to get accurate info up to the city level. |