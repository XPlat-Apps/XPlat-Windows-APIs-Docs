# IGeocoordinate interface

> Namespace: XPlat.Device.Geolocation

Contains the information for identifying a geographic location.

```csharp
public interface IGeocoordinate
```

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