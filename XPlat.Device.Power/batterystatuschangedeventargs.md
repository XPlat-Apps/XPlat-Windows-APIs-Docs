# BatteryStatusChangedEventArgs class

> Namespace: XPlat.Device.Power

Defines an event argument for when the battery status changes.

```csharp
public class BatteryStatusChangedEventArgs : EventArgs
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Constructors

### BatteryStatusChangedEventArgs(BatteryStatus, int)

#### Parameters
##### batteryStatus (BatteryStatus)
The status of the battery.

##### remainingChargePercent (int)
The remaining battery charge as a percentage.

## Properties

### BatteryStatus

Gets the status of the battery.

```csharp
public BatteryStatus BatteryStatus { get; }
```

### RemainingChargePercent

Gets the remaining battery charge as a percentage.

```csharp
public int RemainingChargePercent { get; }
```

### CheckTime

Gets the time the status change check occurred.

```csharp
public DateTime CheckTime { get; }
```