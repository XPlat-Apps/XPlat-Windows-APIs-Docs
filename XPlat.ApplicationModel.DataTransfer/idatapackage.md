# IDataPackage interface

> Namespace: XPlat.ApplicationModel.DataTransfer

Contains the data that a user wants to exchange with another app.

```csharp
public interface IDataPackage
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Methods

### SetText(string)

Sets the text that a DataPackage contains.

```csharp
void SetText(string value)
```

#### Parameters
##### value (string)
The text.