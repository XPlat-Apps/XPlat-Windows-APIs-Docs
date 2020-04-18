# BatteryStatus enum

> Namespace: XPlat.Device.Power

Indicates the status of the battery.

```csharp
public enum BatteryStatus
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
| NotPresent | 0 | The battery or battery controller is not present. |
| Discharging | 1 | The battery is discharging. |
| Idle | 2 | The battery is idle. |
| Charging | 3 | The battery is charging. |