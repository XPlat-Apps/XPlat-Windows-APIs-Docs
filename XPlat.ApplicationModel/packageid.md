# PackageId class

> Namespace: XPlat.ApplicationModel

Provides package identification info, such as name, version, and publisher.

```csharp
public class PackageId : IPackageId
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 |
| UWP | 10.0 | 

## Constructors

### PackageId(Android.Content.PM.PackageInfo) - Android

#### Parameters
##### packageInfo (Android.Content.PM.PackageInfo)
The Android PackageInfo reference to retrieve relevant information from.

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

### Originator - Windows

Gets the original Windows Package reference object.

```csharp
public Windows.ApplicationModel.Package Originator { get; }
```