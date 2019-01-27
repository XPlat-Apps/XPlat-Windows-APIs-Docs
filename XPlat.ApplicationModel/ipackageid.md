# IPackageId interface

> Namespace: XPlat.ApplicationModel

Provides package identification info, such as name, version, and publisher.

```csharp
public interface IPackageId
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Properties

### Name

Gets the name of the package.

```csharp
string Name { get; }
```

### Version

Gets the package version info.

```csharp
PackageVersion Version { get; }
```

### FullName

Gets the full name of the package.

```csharp
string FullName { get; }
```

## Related information

### References

[PackageId - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.packageid)