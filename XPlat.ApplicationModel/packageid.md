# PackageId class

> Namespace: XPlat.ApplicationModel

Provides package identification info, such as name, version, and publisher.

```csharp
public class PackageId : IPackageId
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Constructors

### PackageId(Android.Content.PM.PackageInfo) - Android

#### Parameters
##### packageInfo (Android.Content.PM.PackageInfo)
The Android PackageInfo reference to retrieve relevant information from.

### PackageId(Foundation.NSBundle) - iOS

#### Parameters
##### bundle (Foundation.NSBundle)
The iOS NSBundle reference to retrieve relevant information from.

### PackageId(Windows.ApplicationModel.PackageId) - Windows

#### Parameters
##### packageId (Windows.ApplicationModel.PackageId)
The Windows Package reference to retrieve relevant information from.

## Properties

### Name

Gets the name of the package.

```csharp
public string Name { get; }
```

### Version

Gets the package version info.

```csharp
public PackageVersion Version { get; }
```

### FullName

Gets the full name of the package.

```csharp
public string FullName { get; }
```

### Originator - Android

Gets the original Android PackageInfo reference object.

```csharp
public Android.Content.PM.PackageInfo Originator { get; }
```

### Originator - iOS

Gets the original iOS NSBundle reference object.

```csharp
public Foundation.NSBundle Originator { get; }
```

### Originator - Windows

Gets the original Windows Package reference object.

```csharp
public Windows.ApplicationModel.Package Originator { get; }
```

## Related information

### References

[PackageId - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.packageid)