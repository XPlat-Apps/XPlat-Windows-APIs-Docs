# IGeolocator interface

> Namespace: XPlat.Device.Geolocation

Provides access to the current geographic location.

```csharp
public interface IGeolocator
```

## Properties

### LastKnownPosition

Gets the last known position recorded by the Geolocator.

```csharp
public Geoposition LastKnownPosition { get; }
```

### ReportInterval

Gets or sets the requested minimum time interval between location updates, in milliseconds. If your application requires updates infrequently, set this value so that location services can conserve power by calculating location only when needed.

```csharp
public uint ReportInterval { get; set; }
```

### MovementThreshold

Gets or sets the distance of movement, in meters, relative to the coordinate from the last PositionChanged event, that is required for the Geolocator to raise a PositionChanged event.

```csharp
public double MovementThreshold { get; set; }
```

### LocationStatus

Gets the status that indicates the ability of the Geolocator to provide location updates.

```csharp
public PositionStatus LocationStatus { get; }
```

### DesiredAccuracy

Gets or sets the accuracy level at which the Geolocator provides location updates.

```csharp
public PositionAccuracy DesiredAccuracy { get; set; }
```

### DesiredAccuracyInMeters

Gets or sets the desired accuracy in meters for data returned from the location service.

```csharp
public uint DesiredAccuracyInMeters { get; set; }
```

## Methods

### GetGeopositionAsync()

Starts an asynchronous operation to retrieve the current location of the device.

```csharp
public Task<Geoposition> GetGeopositionAsync()
```

#### Returns
An asynchronous operation that, upon completion, returns a Geoposition marking the found location.

### GetGeopositionAsync(TimeSpan, TimeSpan)

Starts an asynchronous operation to retrieve the current location of the device.

```csharp
public Task<Geoposition> GetGeopositionAsync(TimeSpan maximumAge, TimeSpan timeout)
```

#### Parameters
##### maximumAge (TimeSpan)
The maximum acceptable age of cached location data.

##### timeout (TimeSpan)
The timeout.

#### Returns
An asynchronous operation that, upon completion, returns a Geoposition marking the found location.

### RequestAccessAsync()

Requests permission to access location data.

```csharp
public Task<GeolocationAccessStatus> RequestAccessAsync()
```

#### Returns
A GeolocationAccessStatus that indicates if permission to location data has been granted.

## Events

### PositionChanged

Raised when the location is updated.

```csharp
public event TypedEventHandler<IGeolocator, PositionChangedEventArgs> PositionChanged;
```

### StatusChanged

Raised when the ability of the Geolocator to provide updated location changes.

```csharp
public event TypedEventHandler<IGeolocator, StatusChangedEventArgs> StatusChanged;
```