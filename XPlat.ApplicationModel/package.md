# Package class

> Namespace: XPlat.ApplicationModel

Provides information about a package.

```csharp
public class Package : IPackage, IPackage2, IPackage3
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 |
| UWP | 10.0 | 

## Constructors

### Package(Windows.ApplicationModel.Package) - Windows

#### Parameters
##### package (Windows.ApplicationModel.Package)
The Windows Package reference to retrieve relevant information from.

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

### Originator - Windows

Gets the original Windows Package reference object.

```csharp
public Windows.ApplicationModel.Package Originator { get; }
```