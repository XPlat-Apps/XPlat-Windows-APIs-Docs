# CameraCaptureUIVideoCaptureSettings class

> Namespace: XPlat.Media.Capture

Provides settings for capturing photos.

```csharp
public class CameraCaptureUIVideoCaptureSettings : ICameraCaptureUIVideoCaptureSettings
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
public CameraCaptureUIMaxVideoResolution MaxResolution { get; set; }
```

### MaxDurationInSeconds

Determines the maximum duration of a video.

```csharp
public float MaxDurationInSeconds { get; set; }
```

### AllowTrimming

Determines whether or not the video trimming user interface will be enabled.

```csharp
public bool AllowTrimming { get; set; }
```
