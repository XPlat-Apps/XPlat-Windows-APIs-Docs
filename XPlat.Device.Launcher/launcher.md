# Launcher class

> Namespace: XPlat.Device

Starts the default app associated with the specified file or URI.

```csharp
public class Launcher : ILauncher
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 8.1 |
| UWP | 10.0 |

## Constructors

### Launcher()

The default constructor.

### Launcher(Android.Content.Context) - Android

#### Parameters
##### context (Android.Content.Context)
The current Android context.

## Properties

### Context - Android

Gets or sets the Android context to be used for launching an Activity with.

```csharp
public Context Context { get; set; }
```

## Methods

### LaunchFolderAsync(IStorageFolder)

Launches a file explorer and displays the contents of the specified folder.

```csharp
public Task<bool> LaunchFolderAsync(IStorageFolder folder);
```

#### Parameters
##### folder (IStorageFolder)
The folder to display in a file explorer.

#### Returns
The result of the operation.

### LaunchUriAsync(Uri)

Launches a web browser and displays the contents of the specified URI.

```csharp
public Task<bool> LaunchUriAsync(Uri uri);
```

#### Parameters
##### uri (Uri)
The URI.

#### Returns
Returns true if the default app for the URI scheme was launched; false otherwise.

### QueryUriSupportAsync(Uri)

Asynchronously query whether an app can be activated for the specified URI.

```csharp
public Task<LaunchQuerySupportStatus> QueryUriSupportAsync(Uri uri);
```

#### Parameters
##### uri (Uri)
The URI for which to query support.

#### Returns
A value that indicates whether an application is available to launch the URI.

### LaunchFileAsync(IStorageFile)

Starts the default app associated with the specified file.

```csharp
public Task<bool> LaunchFileAsync(IStorageFile file);
```

#### Parameters
##### file (IStorageFile)
The file.

#### Returns
The launch operation.