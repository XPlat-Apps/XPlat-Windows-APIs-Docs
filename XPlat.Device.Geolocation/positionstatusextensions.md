# PositionStatusExtensions class

> Namespace: XPlat.Device.Geolocation.Extensions

Defines a collection of extensions for the PositionStatus enum.

```csharp
public static class PositionStatusExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Static Methods

### ToInternalPositionStatus(this Windows.Devices.Geolocation.PositionStatus) - Windows

Converts the Windows PositionStatus enum to the internal XPlat equivalent.

```csharp
public static PositionStatus ToInternalPositionStatus(this Windows.Devices.Geolocation.PositionStatus status)
```

#### Parameters
##### status (Windows.Devices.Geolocation.PositionStatus)
The Windows PositionStatus to convert.

#### Returns
Returns the equivalent XPlat PositionStatus value.

### ToWindowsPositionStatus(this PositionStatus) - Windows

Converts the XPlat PositionStatus enum to the Windows equivalent.

```csharp
public static Windows.Devices.Geolocation.PositionStatus ToWindowsPositionStatus(this PositionStatus status)
```

#### Parameters
##### status (Windows.Devices.Geolocation.GeolocationAccessStatus)
The XPlat PositionStatus to convert.

#### Returns
Returns the equivalent Windows PositionStatus value.