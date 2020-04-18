# CameraCaptureUI class

> Namespace: XPlat.Media.Capture

Provides a full window UI for capturing video and photos from a camera.

```csharp
public class CameraCaptureUI
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| UWP | 10.0.16299 | 

## Example

This example shows how to use the CameraCaptureUI class to take a picture. 

```csharp
CameraCaptureUI dialog = new CameraCaptureUI();
dialog.PhotoSettings.MaxResolution = CameraCaptureUIMaxPhotoResolution.HighestAvailable;

IStorageFile file = await dialog.CaptureFileAsync(CameraCaptureUIMode.Photo);
```

## Constructors

### CameraCaptureUI(Android.Content.Context) - Android

#### Parameters
##### context (Android.Content.Context)

The application context.

## Properties

### Context - Android

Gets or sets the Android context to be used for handling activity and intent events.

```csharp
public Android.Content.Context Android { get; set; }
```

### PhotoSettings

Provides settings for capturing photos.

```csharp
public CameraCaptureUIPhotoCaptureSettings PhotoSettings { get; }
```

### VideoSettings

Provides settings for capturing videos. The settings include maximum resolution, maximum duration, and whether or not to allow trimming.

```csharp
public CameraCaptureUIVideoCaptureSettings VideoSettings { get; }
```

## Methods

### CaptureFileAsync(CameraCaptureUIMode)

Launches the CameraCaptureUI user interface.

```csharp
public Task<IStorageFile> CaptureFileAsync(CameraCaptureUIMode mode);
```

#### Parameters
##### mode (CameraCaptureUIMode)
Specifies whether the user interface that will be shown allows the user to capture a photo, capture a video, or capture both photos and videos.

#### Returns
When this operation completes, an IStorageFile object is returned.