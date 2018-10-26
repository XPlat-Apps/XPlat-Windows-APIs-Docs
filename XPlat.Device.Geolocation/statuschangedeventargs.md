# StatusChangedEventArgs class

> Namespace: XPlat.Device.Geolocation

Provides information for the StatusChanged event.

```csharp
public class StatusChangedEventArgs : IStatusChangedEventArgs
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Constructors

### StatusChangedEventArgs(PositionStatus)

#### Parameters
##### status (PositionStatus)
The position status.

### StatusChangedEventArgs(Windows.Devices.Geolocation.PositionStatus) - Windows

#### Parameters
##### status (Windows.Devices.Geolocation.PositionStatus)
The Windows PositionStatus.

### StatusChangedEventArgs(Windows.Devices.Geolocation.StatusChangedEventArgs) - Windows

#### Parameters
##### eventArgs (Windows.Devices.Geolocation.StatusChangedEventArgs)
The Windows StatusChangedEventArgs.

## Properties

### Status

Gets the updated status of the Geolocator object.

```csharp
public PositionStatus Status { get; }
```
