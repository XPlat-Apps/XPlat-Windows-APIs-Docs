# DispatcherTimer class

> Namespace: XPlat.UI

Provides a timer that is integrated into the Dispatcher queue, which is processed at a specified interval of time and at a specified priority.

```csharp
public class DispatcherTimer : IDispatcherTimer
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

NOTE: DispatcherTimer can be accessed from a .NET Standard library, however, it will not run the action on the appropriate platform specific dispatcher. Instead, it will run like a regular System.Threading.Timer.

## Constructors

### DispatcherTimer() - Windows

### DispatcherTimer(Windows.UI.Core.CoreDispatcher) - Windows

#### Parameters
##### dispatcher (Windows.UI.Core.CoreDispatcher)
The Windows CoreDispatcher reference to use the UI thread from to run the tick event.

### DispatcherTimer(UIKit.UIViewController) - iOS

#### Parameters
##### viewController (UIKit.UIViewController)
The iOS UIViewController reference to use the UI thread from to run the tick event.

### DispatcherTimer(Android.App.Activity) - Android

#### Parameters
##### activity (Android.App.Activity)
The Android Activity reference to use the UI thread from to run the tick event.

## Events

### Tick

Occurs when the timer interval has elapsed.

```csharp
public event EventHandler<object> Tick;
```

## Properties

### Dispatcher - Windows

Gets or sets the original Windows CoreDispatcher reference object.

```csharp
public Windows.UI.Core.CoreDispatcher Dispatcher { get; set; }
```

### ViewController - iOS

Gets or sets the original iOS UIViewController reference object.

```csharp
public UIKit.UIViewController ViewController { get; set; }
```

### Activity - Android

Gets or sets the original Android Activity reference object.

```csharp
public Android.App.Activity Activity { get; set; }
```

### Interval

Gets or sets the amount of time between timer ticks.

```csharp
public TimeSpan Interval { get; set; }
```

### IsEnabled

Gets a value indicating whether the timer is running.

```csharp
public bool IsEnabled { get; }
```

## Methods

### Start()

Starts the DispatcherTimer.

```csharp
public void Start();
```

### Stop()

Stops the DispatcherTimer.

```csharp
public void Stop();
```

## Related information

### References

[DispatcherTimer - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.ui.xaml.dispatchertimer)