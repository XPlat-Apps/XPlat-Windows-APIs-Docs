# DataPackageView class

> Namespace: XPlat.ApplicationModel.DataTransfer

A read-only version of a DataPackage. Apps that receive shared content get this object when acquiring content.

```csharp
public class DataPackageView : DataPackage, IDataPackageView
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Methods

### Task<string> GetTextAsync()

Gets the text in the DataPackageView object.

```csharp
public Task<string> GetTextAsync();
```

#### Returns
The text.

## Related information

### References

[DataPackageView - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.datatransfer.datapackageview)