# Geopoint class

> Namespace: XPlat.Device.Geolocation

Describes a geographic point.

```csharp
public class Geopoint : IGeopoint
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Constructors

### Geopoint(BasicGeoposition)

#### Parameters
##### position (BasicGeoposition)
The position.

### Geopoint(Windows.Devices.Geolocation.Geopoint) - Windows

#### Parameters
##### geopoint (Windows.Devices.Geolocation.Geopoint)
The Windows Geopoint.

### Geopoint(Android.Locations.Location) - Android

#### Parameters
##### location (Android.Locations.Location)
The Android Location.

### Geopoint(CoreLocation.CLLocation) - iOS

#### Parameters
##### location (CoreLocation.CLLocation)
The iOS CLLocation.

## Properties

### Position

Gets or sets the position of a geographic point.

```csharp
public BasicGeoposition Position { get; set; }
```
