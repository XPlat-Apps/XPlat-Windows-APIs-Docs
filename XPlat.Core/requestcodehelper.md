# RequestCodeHelper class

> Namespace: XPlat.Helpers

Represents a helper for generating request codes for applications.

```csharp
public static class RequestCodeHelper
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Static Properties

### LastRequestCode

Gets the last requested code.

```csharp
public static int LastRequestCode { get; }
```

## Static Methods

### GenerateRequestCode()

Generates an integer request code.

```csharp
public static int GenerateRequestCode()
```

#### Returns
Returns a value ranging from 1 to 65535 (ushort.MaxValue).

### Reset()

Resets the request code.

```csharp
public static void Reset()
```