# DataPackage class

> Namespace: XPlat.ApplicationModel.DataTransfer

Contains the data that a user wants to exchange with another app.

```csharp
public class DataPackage
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### Originator - Windows

Gets the originating Windows DataPackage instance.

```csharp
public Windows.ApplicationModel.DataTransfer.DataPackage Originator { get; }
```

## Methods

### SetText(string)

Sets the text that a DataPackage contains.

```csharp
public void SetText(string value)
```

#### Parameters
##### value (string)
The text.

## Related information

### References

[DataPackage - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.datatransfer.datapackage)