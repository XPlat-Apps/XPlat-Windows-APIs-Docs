# NSObjectExtensions class

> Namespace: XPlat.Extensions

Defines a collection of extensions for NSObject objects.

```csharp
public static class NSObjectExtensions
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.iOS  | 1.0 |

## Static Methods

### ToObject(this NSObject)

Takes a base NSObject and, depending on it's actual type, will convert the iOS object to a .NET equivalent.

```csharp
public static object ToObject(this NSObject obj)
```

#### Example

This example shows how the ToObject method can be used to convert a stored value from the iOS NSUserDefaults to the .NET equivalent object.

```csharp
public bool TryGetValue(string key, out object value)
{
    NSObject nsObj = null;
    if (!this.ContainsKey(key))
    {
        value = null;
    }
    else
    {
        lock (this.obj)
        {
            // Retrieve a value key from the NSUserDefaults instance.
            nsObj = this.standardUserDefaults.ValueForKey(new NSString(key));
        }

        // Converts the NSObject to the relevant .NET equivalent.
        value = nsObj.ToObject();
    }

    return nsObj != null;
}
```

#### Parameters
##### obj (NSObject)
The iOS object to convert to a .NET object.

#### Returns
Returns the converted .NET object value.