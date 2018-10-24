# BasicGeoposition struct

> Namespace: XPlat.Devices.Geolocation

The basic information to describe a geographic position.

```csharp
public struct BasicGeoposition
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 |

## Fields

### Latitude

The latitude of the geographic position. The valid range of latitude values is from -90.0 to 90.0 degrees.

```csharp
public double Latitude;
```

### Longitude

The longitude of the geographic position. The valid range of longitude values is from -180.0 to 180.0 degrees.

```csharp
public double Longitude;
```

### Altitude

The altitude of the geographic position in meters.

```csharp
public double Altitude;
```

## Constructors

### BasicGeoposition(double, double, double)

#### Parameters
##### latitude (double)
The latitude of the geographic position.

##### longitude (double)
The longitude of the geographic position.

##### altitude (double)
The altitude of the geographic position.

### BasicGeoposition(Windows.Devices.Geolocation.BasicGeoposition) - Windows

#### Parameters
##### geoposition (Windows.Devices.Geolocation.BasicGeoposition)
The Windows BasicGeoposition which will be used to populate the field values.

### BasicGeoposition(Android.Locations.Location) - Android

#### Parameters
##### location (Android.Locations.Location)
The Android Location which will be used to populate the field values.

### BasicGeoposition(CoreLocation.CLLocation) - iOS

#### Parameters
##### location (CoreLocation.CLLocation)
The iOS CLLocation which will be used to populate the field values.