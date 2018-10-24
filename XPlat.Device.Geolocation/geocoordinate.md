# Geocoordinate class

> Namespace: XPlat.Device.Geolocation

Contains the information for identifying a geographic location.

```csharp
public class Geocoordinate : IGeocoordinate
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 |

## Constructors

### Geocoordinate()

Default constructor.

### Geocoordinate(Windows.Devices.Geolocation.Geocoordinate) - Windows

#### Parameters
##### coordinate (Windows.Devices.Geolocation.Geocoordinate)
The Windows Geocoordinate which will be used to populate the field values.

### Geocoordinate(Android.Locations.Location) - Android

#### Parameters
##### location (Android.Locations.Location)
The Android Location which will be used to populate the field values.

### Geocoordinate(CoreLocation.CLLocation) - iOS

#### Parameters
##### location (CoreLocation.CLLocation)
The iOS CLLocation which will be used to populate the field values.

## Properties

### Latitude

Gets or sets the latitude in degrees. The valid range of values is from -90.0 to 90.0.

```csharp
public double Latitude { get; set; }
```

### Longitude

Gets or sets the longitude in degrees. The valid range of values is from -180.0 to 180.0.

```csharp
public double Longitude { get; set; }
```

### Altitude

Gets or sets the altitude of the location, in meters.

```csharp
public double Altitude { get; set; }
```

### Accuracy

Gets or sets the accuracy of the location in meters.

```csharp
public double Accuracy { get; set; }
```

### Heading

Gets or sets the current heading in degrees relative to true north.

```csharp
public double Heading { get; set; }
```

### Speed

Gets or sets the speed in meters per second.

```csharp
public double Speed { get; set; }
```

### Timestamp

Gets or sets the system time at which the location was determined.

```csharp
public DateTimeOffset Timestamp { get; set; }
```

### Point

Gets or sets the location of the Geocoordinate.

```csharp
public Geopoint Point { get; set; }
```