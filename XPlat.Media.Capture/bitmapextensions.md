# BitmapExtensions class

> Namespace: XPlat.Media.Capture.Extensions

Defines a collection of extensions for Bitmaps.

```csharp
public static class BitmapExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Static Methods

### SaveBitmapAsFileAsync(this Android.Graphics.Bitmap, IStorageFolder, string, Android.Graphics.Bitmap.CompressFormat) - Android

Saves an Android Bitmap to an IStorageFile at the specified StorageFolder location by the specified file name.

```csharp
public static async Task<IStorageFile> SaveBitmapAsFileAsync(this Android.Graphics.Bitmap image, IStorageFolder saveLocation, string fileName, Android.Graphics.Bitmap.CompressFormat compressionFormat)
```

#### Example

This example shows how the Take method can be used to take a range of items from a collection.

```csharp
IStorageFile imageFile = await this.bitmap.SaveBitmapAsFileAsync(ApplicationData.Current.LocalFolder, "image.jpg", Bitmap.CompressFormat.Jpeg);
```

#### Parameters
##### image (Android.Graphics.Bitmap)
The image to save.
##### saveLocation (IStorageFolder)
The location to save the file.
##### fileName (string)
The file name (should include the extension).
##### compressionFormat (Android.Graphics.Bitmap.CompressFormat)
The compression format.

#### Returns
When this method completes, it returns the stored image file.