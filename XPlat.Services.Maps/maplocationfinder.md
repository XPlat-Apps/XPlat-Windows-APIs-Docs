# MapLocationFinder class

> Namespace: XPlat.Services.Maps

Provides methods to convert addresses to geographic locations (geocoding) and to convert geographic locations to addresses (reverse geocoding).

```csharp
public static class MapLocationFinder
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Example

This example shows how to convert a geographic location to an address (reverse geocoding).

```csharp
using XPlat.Services.Maps;
...

private async void OnReverseGeocodeButtonClick(object sender, RoutedEventArgs e)
{
    // The location to reverse geocode.
    var location = new XPlat.Device.Geolocation.BasicGeoposition { Latitude = 47.643, Longitude = -122.131 };
    var pointToReverseGeocode = new XPlat.Device.Geolocation.Geopoint(location);

    // Reverse geocode the specified geographic location.
    XPlat.Services.Maps.MapLocationFinderResult result =
        await XPlat.Services.Maps.MapLocationFinder.FindLocationsAtAsync(pointToReverseGeocode);

    // If the query returns results, display the address of the first result.
    if (result.Status == XPlat.Services.Maps.MapLocationFinderStatus.Success)
    {
    System.Diagnostics.Debug.WriteLine($"Address - {result.Locations[0].Address}");
    }
}
```

## Static Methods

### Task<MapLocationFinderResult> FindLocationsAtAsync(Geopoint)

Converts a geopoint to a collection of addresses (reverse geocoding).

```csharp
public static Task<MapLocationFinderResult> FindLocationsAtAsync(Geopoint queryPoint)
```

#### Parameters
##### queryPoint (Geopoint)
The point for which you want to get locations.

#### Returns
When this method completes successfully, it returns a list of locations contained in the MapLocationFinderResult.

### Task<MapLocationFinderResult> FindLocationsAtAsync(Geopoint, MapLocationDesiredAccuracy)

Converts a geopoint to a collection of addresses with the desired accuracy (reverse geocoding).

```csharp
public static Task<MapLocationFinderResult> FindLocationsAtAsync(Geopoint queryPoint, MapLocationDesiredAccuracy accuracy)
```

#### Parameters
##### queryPoint (Geopoint)
The point for which you want to get locations.

##### accuracy (MapLocationDesiredAccuracy)
The desired accuracy for which you want to get locations.

#### Returns
When this method completes successfully, it returns a list of locations contained in the MapLocationFinderResult.

## Related information

### References

[Perform geocoding and reverse geocoding - Microsoft Docs](https://docs.microsoft.com/en-gb/windows/uwp/maps-and-location/geocoding)

[MapLocationFinder - Microsoft Docs](https://docs.microsoft.com/en-gb/uwp/api/Windows.Services.Maps.MapLocationFinder)