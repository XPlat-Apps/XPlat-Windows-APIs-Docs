# Package class

> Namespace: XPlat.ApplicationModel

Provides information about a package.

```csharp
public class Package : IPackage, IPackage2, IPackage3
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Remarks

Use the [Package.Current](#Current) property to get the package for the current app.

## Constructors

### Package(Foundation.NSBundle) - iOS

#### Parameters
##### bundle (Foundation.NSBundle)
The iOS NSBundle reference to retrieve relevant information from.

### Package(Windows.ApplicationModel.Package) - Windows

#### Parameters
##### package (Windows.ApplicationModel.Package)
The Windows Package reference to retrieve relevant information from.

## Static Properties

### Current

Gets the package for the current app.

```csharp
public static Package Current { get; }
```

## Properties

### Id

Gets the package identity of the current package.

```csharp
public IPackageId Id { get; }
```

### InstalledLocation

Gets the location of the installed package.

```csharp
public IStorageFolder InstalledLocation { get; }
```

### Dependencies

Gets the packages on which the current package depends.

```csharp
public IReadOnlyList<IPackage> Dependencies { get; }
```

### DisplayName

Gets the display name of the package.

```csharp
public string DisplayName { get; }
```

### Logo

Gets the logo of the package.

```csharp
public Uri Logo { get; }
```

### IsDevelopmentMode

Indicates whether the package is installed in development mode.

```csharp
public bool IsDevelopmentMode { get; }
```

### InstalledDate

Gets the date on which the application package was installed or last updated.

```csharp
public DateTimeOffset InstalledDate { get; }
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

[Package - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.package)