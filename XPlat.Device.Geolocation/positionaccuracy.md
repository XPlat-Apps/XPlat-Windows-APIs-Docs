# PositionAccuracy enum

> Namespace: XPlat.Device.Geolocation

Indicates the requested accuracy level for the location data that the application uses.

```csharp
public enum PositionAccuracy
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 |

## Fields

| Enum Value | Int Value | Description |
| --- | --- | --- |
| Default | 0 | Optimize for power, performance, and other cost considerations. |
| High | 1 | Deliver the most accurate report possible. This includes using services that might charge money, or consuming higher levels of battery power or connection bandwidth. An accuracy level of High may degrade system performance and should be used only when necessary. |
