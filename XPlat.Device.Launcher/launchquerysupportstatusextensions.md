# LaunchQuerySupportStatusExtensions class

> Namespace: XPlat.Device.Extensions

Defines a collection of extensions for the LaunchQuerySupportStatus enum.

```csharp
public static class LaunchQuerySupportStatusExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Static Methods

### ToInternalLaunchQuerySupportStatus(this Windows.System.LaunchQuerySupportStatus) - Windows

Converts the Windows LaunchQuerySupportStatus enum to the internal XPlat equivalent.

```csharp
public static LaunchQuerySupportStatus ToInternalLaunchQuerySupportStatus(
    this Windows.System.LaunchQuerySupportStatus status)
```

#### Parameters
##### status (Windows.System.LaunchQuerySupportStatus)
The Windows LaunchQuerySupportStatus to convert.

#### Returns
Returns the equivalent XPlat LaunchQuerySupportStatus value.

### ToWindowsLaunchQuerySupportStatus(this LaunchQuerySupportStatus) - Windows

Converts the XPlat LaunchQuerySupportStatus enum to the Windows equivalent.

```csharp
public static LaunchQuerySupportStatus ToWindowsLaunchQuerySupportStatus(this LaunchQuerySupportStatus status)
```

#### Parameters
##### status (LaunchQuerySupportStatus)
The XPlat LaunchQuerySupportStatus to convert.

#### Returns
Returns the equivalent Windows LaunchQuerySupportStatus value.