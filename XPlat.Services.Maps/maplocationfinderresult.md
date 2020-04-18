# MapLocationFinderResult class

> Namespace: XPlat.Services.Maps

Returns the result of a MapLocationFinder query.

```csharp
public class MapLocationFinderResult
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Constructors

### MapLocationFinderResult(Windows.Services.Maps.MapLocationFinderResult) - Windows

#### Parameters
##### result (Windows.Services.Maps.MapLocationFinderResult)

### MapLocationFinderResult(IEnumerable<Android.Locations.Address>, MapLocationFinderStatus) - Android

#### Parameters
##### result (IEnumerable<Android.Locations.Address>)

##### status (MapLocationFinderStatus)

### MapLocationFinderResult(CoreLocation.CLPlacemark[], MapLocationFinderStatus) - iOS

#### Parameters
##### result (CoreLocation.CLPlacemark[])

##### status (MapLocationFinderStatus)

## Properties

### Locations

Gets the list of locations found by a MapLocationFinder query.

```csharp
public IReadOnlyList<XPlat.Services.Maps.MapLocation> Locations { get; }
```

### Status

Gets the status of a MapLocationFinder query.

```csharp
public XPlat.Services.Maps.MapLocationFinderStatus Status { get; }
```