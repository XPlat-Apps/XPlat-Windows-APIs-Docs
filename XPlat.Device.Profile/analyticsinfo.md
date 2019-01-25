# AnalyticsInfo class

> Namespace: XPlat.Device.Profile

Provides information about the device for profiling purposes.

```csharp
public static class AnalyticsInfo
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Static Properties

### VersionInfo

Gets version info about the device family.

```csharp
public static AnalyticsVersionInfo VersionInfo { get; }
```

### DeviceForm

Gets the device form factor. For example, the app could be running on a phone, tablet, desktop, and so on.

```csharp
public static string DeviceForm { get; }
```

#### Remarks

The `DeviceForm` property returns the following values for the following platforms:

##### Android

* `Desktop` - When the current device family is Desktop
* `Car` - When the current device family is Auto
* `Mobile` - When the current device family is Mobile
* `Tablet` - When the current device family is Tablet
* `Television` - When the current device family is TV
* `Wearable` - When the current device family is VR or Wear

##### iOS

* `Desktop` - When the current device family is MacOS
* `Car` - When the current device family is CarPlay
* `Mobile` - When the current device family is iPhone
* `Tablet` - When the current device family is iPad
* `Television` - When the current device family is TV
* `Wearable` - When the current device family is Watch

##### Windows

* `Desktop` - When the current device family is Desktop
* `Phone` - When the current device family is Phone
* `Tablet` - When the current device family is Tablet
* `Surface Hub` - When the current device family is Surface Hub
* `Head-mounted display` - When the current device family is HMD