# IDataPackageView interface

> Namespace: XPlat.ApplicationModel.DataTransfer

A read-only version of a DataPackage. Apps that receive shared content get this object when acquiring content.

```csharp
public interface IDataPackageView
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Methods

### Task<string> GetTextAsync()

Gets the text in the DataPackageView object.

```csharp
Task<string> GetTextAsync();
```

#### Returns
The text.