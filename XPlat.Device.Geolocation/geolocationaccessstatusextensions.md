# GeolocationAccessStatusExtensions class

> Namespace: XPlat.Device.Geolocation.Extensions

Defines a collection of extensions for the GeolocationAccessStatus enum.

```csharp
public static class GeolocationAccessStatusExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Static Methods

### ToInternalGeolocationAccessStatus(this Windows.Devices.Geolocation.GeolocationAccessStatus) - Windows

Converts the Windows GeolocationAccessStatus enum to the internal XPlat equivalent.

```csharp
public static GeolocationAccessStatus ToInternalGeolocationAccessStatus(
    this Windows.Devices.Geolocation.GeolocationAccessStatus status)
```

#### Parameters
##### status (Windows.Devices.Geolocation.GeolocationAccessStatus)
The Windows GeolocationAccessStatus to convert.

#### Returns
Returns the equivalent XPlat GeolocationAccessStatus value.

### ToWindowsGeolocationAccessStatus(this GeolocationAccessStatus) - Windows

Converts the XPlat GeolocationAccessStatus enum to the Windows equivalent.

```csharp
public static Windows.Devices.Geolocation.GeolocationAccessStatus ToWindowsGeolocationAccessStatus(
    this GeolocationAccessStatus status)
```

#### Parameters
##### status (Windows.Devices.Geolocation.GeolocationAccessStatus)
The XPlat GeolocationAccessStatus to convert.

#### Returns
Returns the equivalent Windows GeolocationAccessStatus value.