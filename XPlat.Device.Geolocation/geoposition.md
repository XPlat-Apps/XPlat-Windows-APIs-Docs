# Geoposition class

> Namespace: XPlat.Device.Geolocation

Represents a location that may contain latitude and longitude data.

```csharp
public class Geoposition : IGeoposition
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Constructors

### Geoposition()

The default constructor.

### Geoposition(Geocoordinate)

#### Parameters
##### coordinate (Geocoordinate)
The coordinate.

### Geoposition(Windows.Devices.Geolocation.Geocoordinate) - Windows

#### Parameters
##### coordinate (Windows.Devices.Geolocation.Geocoordinate)
The Windows Geocoordinate.

### Geoposition(Windows.Devices.Geolocation.Geoposition) - Windows

#### Parameters
##### position (Windows.Devices.Geolocation.Geoposition)
The Windows Geoposition.

### Geoposition(Android.Locations.Location) - Android

#### Parameters
##### location (Android.Locations.Location)
The Android Location.

### Geoposition(CoreLocation.CLLocation) - iOS

#### Parameters
##### location (CoreLocation.CLLocation)
The iOS CLLocation.

## Properties

### Coordinate

Gets or sets the latitude and longitude associated with a geographic location.

```csharp
public Geocoordinate Coordinate { get; set; }
```
