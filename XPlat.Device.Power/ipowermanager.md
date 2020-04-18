# IPowerManager interface

> Namespace: XPlat.Device.Power

Provides access to information about a device's battery and power supply status.

```csharp
public interface IPowerManager
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### BatteryStatus

Gets the device's battery status.

```csharp
BatteryStatus BatteryStatus { get; }
```

### RemainingChargePercent

Gets the total percentage of charge remaining from all batteries connected to the device.

```csharp
int RemainingChargePercent { get; }
```

## Events

### BatteryStatusChanged

Occurs when BatteryStatus changes.

```csharp
event EventHandler<BatteryStatus> BatteryStatusChanged;
```

### RemainingChargePercentChanged

Occurs when RemainingChargePercent changes.

```csharp
event EventHandler<int> RemainingChargePercentChanged;
```