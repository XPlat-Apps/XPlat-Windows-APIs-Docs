# IAnalyticsVersionInfo interface

> Namespace: XPlat.Device.Profile

Provides version information about the device family.

```csharp
public interface IAnalyticsVersionInfo
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### DeviceFamily

Gets a string that represents the type of device the application is running on.

```csharp
string DeviceFamily { get; }
```

### DeviceFamilyVersion

Gets the version within the device family.

```csharp
string DeviceFamilyVersion { get; }
```