# IMapLocationFinderResult interface

> Namespace: XPlat.Services.Maps

Returns the result of a MapLocationFinder query.

```csharp
public interface IMapLocationFinderResult
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### Locations

Gets the list of locations found by a MapLocationFinder query.

```csharp
IReadOnlyList<XPlat.Services.Maps.MapLocation> Locations { get; }
```

### Status

Gets the status of a MapLocationFinder query.

```csharp
XPlat.Services.Maps.MapLocationFinderStatus Status { get; }
```