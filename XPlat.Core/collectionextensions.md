# CollectionExtensions class

> Namespace: XPlat.Extensions

Defines a collection of extensions for enumerable objects.

```csharp
public static class CollectionExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Static Methods

### Take<T>(this List<T>, int, int)

Takes a number of elements from the specified list from the specified starting index.

```csharp
public static IEnumerable<T> Take<T>(this List<T> list, int startingIndex, int takeCount)
```

#### Parameters
##### list (List)
The list to take items from.
##### startingIndex (int)
The index to start at in the list.
##### takeCount (int)
The number of items to take from the starting index of the list.

#### Returns
Returns a collection of T items.

### Take<T>(this IReadOnlyList<T>, int, int)

Takes a number of elements from the specified readonly list from the specified starting index.

```csharp
public static IEnumerable<T> Take<T>(this IReadOnlyList<T> list, int startingIndex, int takeCount)
```

#### Example

This example shows how the Take method can be used to take a range of items from a collection.

```csharp
IReadOnlyList<IStorageItem> items = await this.GetItemsAsync();

/// Gets the 5th to 10th items.
List<IStorageItem> specificItems = items.Take(5, 10).ToList();
```

#### Parameters
##### list (List)
The list to take items from.
##### startingIndex (int)
The index to start at in the list.
##### takeCount (int)
The number of items to take from the starting index of the list.

#### Returns
Returns a collection of T items.