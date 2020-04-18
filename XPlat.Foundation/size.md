# Size struct

> Namespace: XPlat.Foundation

Represents number values that specify a height and width.

```csharp
public struct Size
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 |

## Constructors

### Size(double, double)

#### Parameters
##### width (double)

##### height (double)

## Static Properties

### Empty

Gets a value that represents an empty Size.

```csharp
public static Size Empty { get; }
```

## Properties

### Width

The width. 

```csharp
public double Width { get; set; }
```

### Height

The height.

```csharp
public double Height { get; set; }
```

### IsEmpty

Gets a value that indicates whether this instance of Size is Empty.

```csharp
public bool IsEmpty { get; }
```