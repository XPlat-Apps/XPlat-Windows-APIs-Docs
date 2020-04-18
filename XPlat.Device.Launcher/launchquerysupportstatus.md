# LaunchQuerySupportStatus enum

> Namespace: XPlat.Device

Specifies whether an app is available that supports activation.

```csharp
public enum LaunchQuerySupportStatus
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Fields

| Enum Value | Int Value | Description |
| --- | --- | --- |
| Available | 0 | An app that handles the activation is available and may be activated. |
| AppNotInstalled | 1 | No app is installed to handle the activation. |
| AppUnavailable | 2 | An app that handles the activation is installed but not available because it is being updated by the store or it was installed on a removable device that is not available. |
| NotSupported | 3 | The app does not handle the activation. |
| Unknown | 4 | An unknown error was encountered while determining whether an app supports the activation. |
