# CameraCaptureUIMode enum

> Namespace: XPlat.Media.Capture

Determines whether the user interface for capturing from the attached camera allows capture of photos, videos, or both photos and videos.

```csharp
public enum CameraCaptureUIMode
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Fields

| Enum Value | Int Value | Description |
| --- | --- | --- |
| PhotoOrVideo | 0 | Either a photo or video can be captured. |
| Photo | 1 | The user can only capture a photo. |
| Video | 2 | The user can only capture a video. |