# PositionStatus enum

> Namespace: XPlat.Device.Geolocation

Indicates the ability of the Geolocator object to provide location data.

```csharp
public enum PositionStatus
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 |

## Fields

| Enum Value | Int Value | Description |
| --- | --- | --- |
| Ready | 0 | Location data is available. |
| Initializing | 1 | Location services is initializing. This is the status if a GPS is the source of location data and the GPS receiver does not yet have the required number of satellites in view to obtain an accurate position. |
| NoData | 2 | No location data is available from any source. LocationStatus will have this value if the application calls GetGeopositionAsync or registers an event handler for the PositionChanged event, before data is available from a location sensor. Once data is available LocationStatus transitions to the Ready state. |
| Disabled | 3 | Location settings are turned off. This status indicates that the user has not granted the application permission to access location. |
| NotInitialized | 4 | An operation to retrieve location has not yet been initialized. LocationStatus will have this value if the application has not yet called GetGeopositionAsync or registered an event handler for the PositionChanged event. LocationStatus may also have this value if your app doesn't have permission to access location. Call the RequestAccessAsync before accessing the user's location. At that time, your app must be in the foreground and RequestAccessAsync must be called from the UI thread. Until the user grants your app permission to their location, your app can't access location data. |
| NotAvailable | 5 | Location services is not available. |
