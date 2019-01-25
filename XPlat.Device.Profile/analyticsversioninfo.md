# AnalyticsVersionInfo class

> Namespace: XPlat.Device.Profile

Provides version information about the device family.

```csharp
public class AnalyticsVersionInfo : IAnalyticsVersionInfo
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Constructors

### AnalyticsVersionInfo(Windows.System.Profile.AnalyticsVersionInfo) - Windows

#### Parameters
##### versionInfo (Windows.System.Profile.AnalyticsVersionInfo)
The Windows AnalyticsVersionInfo reference to retrieve relevant information from.

## Properties

### DeviceFamily

Gets a string that represents the type of device the application is running on.

```csharp
public string DeviceFamily { get; }
```

#### Remarks

The `DeviceFamily` property returns the following values for the following platforms:

##### Android

* `Android.Auto` - When the current UI mode is Car
* `Android.Desktop` - When the current UI mode is Desk
* `Android.Mobile` - When the device type is detected as phone
* `Android.Tablet` - When the device type is detected as tablet
* `Android.TV` - When the current UI mode is Television
* `Android.VR` - When the current UI mode is VR Headset
* `Android.Wear` - When the current UI mode is Watch

##### iOS

* `Apple.CarPlay` - When the current UI mode is CarPlay
* `Apple.iPhone` - When the current UI mode is Phone
* `Apple.iPad` - When the current UI mode is Pad
* `Apple.TV` - When the current UI mode is TV

##### Windows

* `Windows.Desktop` - When the current UI mode is Desktop
* `Windows.Mobile` - When the current UI mode is Mobile
* `Windows.Team` - When the current UI mode is Surface Hub
* `Windows.IoT` - When the current UI mode is IoT
* `Windows.Xbox` - When the current UI mode is Xbox
* `Windows.Holographic` - When the current UI mode is Holographic

### DeviceFamilyVersion

Gets the version within the device family.

```csharp
public string DeviceFamilyVersion { get; }
```