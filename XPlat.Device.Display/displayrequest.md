# DisplayRequest class

> Namespace: XPlat.Device.Display

Represents a display request.

```csharp
public class DisplayRequest : IDisplayRequest
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Example

```csharp
public void Initialize()
{
    this.displayRequest = new DisplayRequest(this.Activity.Window);
    
    try
    {
        // This call activates a display-required request. If successful,  
        // the screen is guaranteed not to turn off automatically due to user inactivity. 
        this.displayRequest.RequestActive();
    }
    catch (Exception ex)
    {
        System.Diagnostics.Debug.WriteLine(ex.ToString());
    }

    // Perform long-running application initialization.

    try
    {
        // This call de-activates the display-required request. If successful, the screen 
        // might be turned off automatically due to a user inactivity, depending on the 
        // power policy settings of the system. 
        this.displayRequest.RequestRelease();
    }
    catch (Exception ex)
    {
        System.Diagnostics.Debug.WriteLine(ex.ToString());
    }
}
```

## Constructors

### DisplayRequest(Android.Views.Window) - Android

#### Parameters
##### currentWindow (Android.Views.Window)
The Window which will be used to request the wake lock.

## Properties

### Originator - Android

Gets the Android Window instance.

```csharp
public Android.Views.Window Originator { get; }
```

### Originator - Windows

Gets the Windows DisplayRequest instance.

```csharp
public Windows.System.Display.DisplayRequest Originator { get; }
```

## Methods

### RequestActive()

Activates a display request.

```csharp
void RequestActive();
```

### RequestRelease()

Deactivates a display request.

```csharp
void RequestRelease();
```
