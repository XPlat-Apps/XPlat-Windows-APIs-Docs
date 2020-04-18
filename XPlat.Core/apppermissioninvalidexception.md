# AppPermissionInvalidException class

> Namespace: XPlat.Exceptions

Defines an exception that is thrown when an application permission is not set.

```csharp
public class AppPermissionInvalidException : Exception
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Constructors

### AppPermissionInvalidException(string, string)

#### Parameters
##### permission (string)
The permission which could not be found.
##### message (string)
The error message that explains the reason for the exception.

### AppPermissionInvalidException(string, string, Exception)

#### Parameters
##### permission (string)
The permission which could not be found.
##### message (string)
The error message that explains the reason for the exception.
##### innerException (Exception)
The exception that is the cause of the current exception.

## Properties

### PermissionCode

Gets the permission which could not be found.

```csharp
public string PermissionCode { get; }
```