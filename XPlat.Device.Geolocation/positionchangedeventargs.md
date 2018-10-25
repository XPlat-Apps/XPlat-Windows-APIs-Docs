# PositionChangedEventArgs class

> Namespace: XPlat.Device.Geolocation

Provides data for the PositionChanged event.

```csharp
public class PositionChangedEventArgs
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 |

## Constructors

### PositionChangedEventArgs(Geoposition)

#### Parameters
##### position (Geoposition)
The location data associated with the PositionChanged event.

### PositionChangedEventArgs(Windows.Devices.Geolocation.PositionChangedEventArgs) - Windows

#### Parameters
##### eventArgs (Windows.Devices.Geolocation.PositionChangedEventArgs)
The Windows PositionChangedEventArgs.

### PositionChangedEventArgs(Windows.Devices.Geolocation.Geoposition) - Windows

#### Parameters
##### position (Windows.Devices.Geolocation.Geoposition)
The Windows Geoposition.

### PositionChangedEventArgs(Android.Locations.Location) - Android

#### Parameters
##### location (Android.Locations.Location)
The Android Location.

### PositionChangedEventArgs(CoreLocation.CLLocation) - iOS

#### Parameters
##### location (CoreLocation.CLLocation)
The iOS CLLocation.

## Properties

### Position

Gets the location data associated with the PositionChanged event.

```csharp
public Geoposition Position { get; }
```