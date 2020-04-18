# PowerManager class

> Namespace: XPlat.Device.Power

Provides access to information about a device's battery and power supply status.

```csharp
public sealed class PowerManager : IPowerManager, IDisposable
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Static Properties

### Current

Gets the current instance of the PowerManager.

```csharp
public static PowerManager Current { get; }
```

## Properties

### BatteryStatus

Gets the device's battery status.

```csharp
public BatteryStatus BatteryStatus { get; }
```

### RemainingChargePercent

Gets the total percentage of charge remaining from all batteries connected to the device.

```csharp
public int RemainingChargePercent { get; }
```

## Events

### BatteryStatusChanged

Occurs when BatteryStatus changes.

```csharp
public event EventHandler<BatteryStatus> BatteryStatusChanged;
```

### RemainingChargePercentChanged

Occurs when RemainingChargePercent changes.

```csharp
public event EventHandler<int> RemainingChargePercentChanged;
```