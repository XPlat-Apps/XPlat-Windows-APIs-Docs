# CollectionChange enum

> Namespace: XPlat.Foundation.Collections

Describes the action that causes a change to a collection.

```csharp
public enum CollectionChange
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
| Reset | 0 | The collection is changed. |
| ItemInserted | 1 | An item is added to the collection. |
| ItemRemoved | 2 | An item is removed from the collection. |
| ItemChanged | 3 | An item is changed in the collection. |