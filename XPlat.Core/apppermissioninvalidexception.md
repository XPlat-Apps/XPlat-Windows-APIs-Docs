# AppPermissionInvalidException class

> Namespace: XPlat.Exceptions

Defines an exception that is thrown when an application permission is not set.

```csharp
public class AppPermissionInvalidException : Exception
```

### Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 1.4 |
| Xamarin.Android | 8.1 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0 | 

## Constructors

### AppPermissionInvalidException(string, string)

#### Parameters
##### permission
The permission which could not be found.
##### message
The error message that explains the reason for the exception.

### AppPermissionInvalidException(string, string, Exception)


#### Parameters
##### permission
The permission which could not be found.
##### message
The error message that explains the reason for the exception.
##### innerException
The exception that is the cause of the current exception.

## Properties

### PermissionCode

Gets the permission which could not be found.

```csharp
public string PermissionCode { get; }
```