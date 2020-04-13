# Clipboard class

> Namespace: XPlat.ApplicationModel.DataTransfer

Gets and sets information from the clipboard object.

```csharp
public static class Clipboard
```

## Supported platforms

| Platform | Version |
| --- | --- |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Example

This example shows how to use the Clipboard class to add text to be pasted anywhere, and retrieve text from the Clipboard.

```csharp
using XPlat.ApplicationModel.DataTransfer;
...

private void CopyNoteTextToClipboard(Note note)
{
    Clipboard.SetText(note.ToString());
}

private async Task CopyTextToNote(Note note)
{
    note.Text = await Clipboard.GetTextAsync();
}
```

## Static Methods

### GetContent()

Gets the current content that is stored in the clipboard object.

```csharp
public static DataPackageView GetContent()
```

#### Returns
Contains the content of the Clipboard.

### GetTextAsync()

Gets the current text content that is stored in the clipboard object.

```csharp
public static async Task<string> GetTextAsync()
```

#### Returns
The text.

### SetContent(DataPackage)

Sets the current content that is stored in the clipboard object.

```csharp
public static void SetContent(DataPackage content)
```

#### Parameters
##### content (DataPackage)
Contains the content of the clipboard. If NULL, the clipboard is emptied.

### SetText(string)

Sets the current text that is stored in the clipboard object.

```csharp
public static void SetText(string text)
```

#### Parameters
##### text (string)
The text.

### Clear()

Removes all data from the Clipboard.

```csharp
public static void Clear()
```

## Static Events

### ContentChanged

Occurs when the data stored in the Clipboard changes.

```csharp
public static event EventHandler<object> ContentChanged;
```

## Related information

### References

[Clipboard - Microsoft Docs](https://docs.microsoft.com/en-us/uwp/api/windows.applicationmodel.datatransfer.clipboard)