# IDisplayRequest interface

> Namespace: XPlat.Device.Display

Represents a display request.

```csharp
public interface IDisplayRequest
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

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