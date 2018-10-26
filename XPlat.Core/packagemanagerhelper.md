# PackageManagerHelper class

> Namespace: XPlat.Helpers

Defines a helper for the Android PackageManager.

```csharp
public static class PackageManagerHelper
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 | 

## Static Methods

### CheckContentProviderExists(string)

Checks whether a content provider exists within the application's registered package manager providers.

```csharp
public static bool CheckContentProviderExists(string providerName)
```

#### Parameters
##### providerName (string)
The name of the provider to check is registered.

#### Returns
Returns a value indicating whether the content provider exists.
