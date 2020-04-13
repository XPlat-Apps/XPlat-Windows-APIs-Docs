# GeolocationAccessStatus enum

> Namespace: XPlat.Device.Geolocation

Indicates if your app has permission to access location data.

```csharp
public enum GeolocationAccessStatus
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
| Unspecified | 0 | Permission to access location was not specified. |
| Allowed | 1 | Permission to access location was granted. |
| Denied | 2 | Permission to access location was denied. |