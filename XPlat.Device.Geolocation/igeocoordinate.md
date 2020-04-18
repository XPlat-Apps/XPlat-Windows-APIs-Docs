# IGeocoordinate interface

> Namespace: XPlat.Device.Geolocation

Contains the information for identifying a geographic location.

```csharp
public interface IGeocoordinate
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Properties

### Latitude

Gets or sets the latitude in degrees. The valid range of values is from -90.0 to 90.0.

```csharp
double Latitude { get; set; }
```

### Longitude

Gets or sets the longitude in degrees. The valid range of values is from -180.0 to 180.0.

```csharp
double Longitude { get; set; }
```

### Altitude

Gets or sets the altitude of the location, in meters.

```csharp
double Altitude { get; set; }
```

### Accuracy

Gets or sets the accuracy of the location in meters.

```csharp
double Accuracy { get; set; }
```

### Heading

Gets or sets the current heading in degrees relative to true north.

```csharp
double Heading { get; set; }
```

### Speed

Gets or sets the speed in meters per second.

```csharp
double Speed { get; set; }
```

### Timestamp

Gets or sets the system time at which the location was determined.

```csharp
DateTimeOffset Timestamp { get; set; }
```

### Point

Gets or sets the location of the Geocoordinate.

```csharp
Geopoint Point { get; set; }
```