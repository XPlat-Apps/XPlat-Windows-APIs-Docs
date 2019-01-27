# IPackage2 interface

> Namespace: XPlat.ApplicationModel

Provides information about a package.

```csharp
public interface IPackage2
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Properties

### DisplayName

Gets the display name of the package.

```csharp
string DisplayName { get; }
```

### Logo

Gets the logo of the package.

```csharp
Uri Logo { get; }
```

### IsDevelopmentMode

Indicates whether the package is installed in development mode.

```csharp
bool IsDevelopmentMode { get; }
```

## Related information

### References

[Package - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.package)