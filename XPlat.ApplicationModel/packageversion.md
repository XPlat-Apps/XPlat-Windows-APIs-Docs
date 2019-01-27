# PackageVersion struct

> Namespace: XPlat.ApplicationModel

Represents the package version info

```csharp
public struct PackageVersion
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 |

## Example

Use the Package.Current property to get the package for the current app. Use the Package.Id property to get the package ID, from which you can then get the version.

```csharp
using XPlat.ApplicationModel;

Package package = Package.Current;
IPackageId packageId = package.Id;
PackageVersion version = packageId.Version;
```

## Fields

### Major

The major version number of the package.

```csharp
public ushort Major;
```

### Minor

The minor version number of the package.

```csharp
public ushort Minor;
```

### Build

The build version number of the package.

```csharp
public ushort Build;
```

### Revision

The revision version number of the package.

```csharp
public ushort Revision;
```

## Related information

### References

[PackageVersion - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.packageversion)