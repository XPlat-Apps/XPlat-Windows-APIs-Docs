# IMapLocation interface

> Namespace: XPlat.Services.Maps

Represents a geographic location.

```csharp
public interface IMapLocation
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### Point

Gets the coordinates of a geographic location.

```csharp
XPlat.Device.Geolocation.Geopoint Point { get; }
```

### DisplayName

Gets the display name of a geographic location.

```csharp
string DisplayName { get; }
```

### Description

Gets the description of a geographic location.

```csharp
string Description { get; }
```

### Address

Gets the address of a geographic location.

```csharp
XPlat.Services.Maps.MapAddress Address { get; }
```