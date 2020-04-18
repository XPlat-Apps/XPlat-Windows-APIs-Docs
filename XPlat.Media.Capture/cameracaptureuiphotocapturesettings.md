# CameraCaptureUIPhotoCaptureSettings class

> Namespace: XPlat.Media.Capture

Provides settings for capturing photos.

```csharp
public class CameraCaptureUIPhotoCaptureSettings : ICameraCaptureUIPhotoCaptureSettings
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### MaxResolution

Determines the maximum resolution the user will be able to select. Default, HighestAvailable.

```csharp
public CameraCaptureUIMaxPhotoResolution MaxResolution { get; set; }
```

### AllowCropping

Determines whether photo cropping will be enabled in the user interface for capture a photo.

```csharp
public bool AllowCropping { get; set; }
```
