# MapLocationFinderStatus enum

> Namespace: XPlat.Services.Maps

Returns the status of a MapLocationFinder query. This enumeration provides values for the Status property of a MapLocationFinderResult.

```csharp
public enum MapLocationFinderStatus
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Fields

| Enum Value | Int Value | Description |
| --- | --- | --- |
| Success | 0 | Query search operation was successful. Check result size before accessing results. |
| UnknownError | 1 | The query returned an unknown error. |
| InvalidCredentials | 2 | The query provided credentials that are not valid. |
| BadLocation | 3 | The specified point cannot be converted to a location. For example, the point is in an ocean or a desert. |
| IndexFailure | 4 | The query encountered an internal error. |
| NetworkFailure | 5 | The query encountered a network failure. |
| NotSupported | 6 | The query is not supported. |