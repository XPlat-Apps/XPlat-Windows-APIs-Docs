# StorageFileExtensions class

> Namespace: XPlat.Media.Capture.Extensions

Defines a collection of extensions for storage files in regards to media capture.

```csharp
public static class StorageFileExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Static Methods

### ResizeImageFileAsync(this IStorageFile, CameraCaptureUIMaxPhotoResolution) - Android

Resizes an image stored in a storage file to the given resolution.

```csharp
public static async Task<IStorageFile> ResizeImageFileAsync(this IStorageFile imageFile, CameraCaptureUIMaxPhotoResolution resolution)
```

#### Example

This example shows how the Take method can be used to take a range of items from a collection.

```csharp
IStorageFile imageFile = await this.bitmap.SaveBitmapAsFileAsync(ApplicationData.Current.LocalFolder, "image.jpg", Bitmap.CompressFormat.Jpeg);

imageFile = await imageFile.ResizeImageFileAsync(CameraCaptureUIMaxPhotoResolution.Large3M);
```

#### Parameters
##### imageFile (IStorageFile)
The image to resize.
##### resolution (CameraCaptureUIMaxPhotoResolution)
The resolution to resize the image to.

#### Returns
When this method completes, it returns the resized image file.