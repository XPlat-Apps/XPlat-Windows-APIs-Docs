# IDispatcherTimer interface

> Namespace: XPlat.UI

Provides a timer that is integrated into the Dispatcher queue, which is processed at a specified interval of time and at a specified priority.

```csharp
public interface IDispatcherTimer
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Events

### Tick

Occurs when the timer interval has elapsed.

```csharp
event EventHandler<object> Tick;
```

## Properties

### Interval

Gets or sets the amount of time between timer ticks.

```csharp
TimeSpan Interval { get; set; }
```

### IsEnabled

Gets a value indicating whether the timer is running.

```csharp
bool IsEnabled { get; }
```

## Methods

### Start()

Starts the DispatcherTimer.

```csharp
void Start();
```

### Stop()

Stops the DispatcherTimer.

```csharp
void Stop();
```

## Related information

### References

[DispatcherTimer - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.dispatchertimer)