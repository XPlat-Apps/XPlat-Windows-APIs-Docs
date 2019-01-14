# IPackage3 interface

> Namespace: XPlat.ApplicationModel

Provides information about a package.

```csharp
public interface IPackage3
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Properties

### InstalledDate

Gets the date on which the application package was installed or last updated.

```csharp
DateTimeOffset InstalledDate { get; }
```