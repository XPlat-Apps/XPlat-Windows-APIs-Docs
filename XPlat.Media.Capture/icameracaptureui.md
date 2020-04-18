# ICameraCaptureUI interface

> Namespace: XPlat.Media.Capture

Provides a full window UI for capturing video and photos from a camera.

```csharp
public interface ICameraCaptureUI
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### PhotoSettings

Provides settings for capturing photos.

```csharp
CameraCaptureUIPhotoCaptureSettings PhotoSettings { get; }
```

### VideoSettings

Provides settings for capturing videos. The settings include maximum resolution, maximum duration, and whether or not to allow trimming.

```csharp
CameraCaptureUIVideoCaptureSettings VideoSettings { get; }
```

## Methods

### CaptureFileAsync(CameraCaptureUIMode)

Launches the CameraCaptureUI user interface.

```csharp
Task<IStorageFile> CaptureFileAsync(CameraCaptureUIMode mode);
```

#### Parameters
##### mode (CameraCaptureUIMode)
Specifies whether the user interface that will be shown allows the user to capture a photo, capture a video, or capture both photos and videos.

#### Returns
When this operation completes, an IStorageFile object is returned.