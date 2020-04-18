# IDisplayRequest interface

> Namespace: XPlat.Device.Display

Represents a display request.

```csharp
public interface IDisplayRequest
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

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