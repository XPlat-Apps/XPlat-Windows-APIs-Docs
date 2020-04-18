# MapLocation class

> Namespace: XPlat.Services.Maps

Represents a geographic location.

```csharp
public class MapLocation
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Constructors

### MapLocation(Windows.Services.Maps.MapLocation) - Windows

#### Parameters
##### mapAddress (Windows.Services.Maps.MapLocation)

### MapLocation(Android.Locations.Address) - Android

#### Parameters
##### mapLocation (Android.Locations.Address)

### MapLocation(CoreLocation.CLPlacemark) - iOS

#### Parameters
##### mapLocation (CoreLocation.CLPlacemark)

## Properties

### Point

Gets the coordinates of a geographic location.

```csharp
public XPlat.Device.Geolocation.Geopoint Point { get; }
```

### DisplayName

Gets the display name of a geographic location.

```csharp
public string DisplayName { get; }
```

### Description

Gets the description of a geographic location.

```csharp
public string Description { get; }
```

### Address

Gets the address of a geographic location.

```csharp
public XPlat.Services.Maps.MapAddress Address { get; }
```