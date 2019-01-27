# IPackage interface

> Namespace: XPlat.ApplicationModel

Provides information about a package.

```csharp
public interface IPackage
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Properties

### Id

Gets the package identity of the current package.

```csharp
IPackageId Id { get; }
```

### InstalledLocation

Gets the location of the installed package.

```csharp
IStorageFolder InstalledLocation { get; }
```

### Dependencies

Gets the packages on which the current package depends.

```csharp
IReadOnlyList<IPackage> Dependencies { get; }
```

## Related information

### References

[Package - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.package)