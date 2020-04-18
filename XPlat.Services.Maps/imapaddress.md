# IMapAddress interface

> Namespace: XPlat.Services.Maps

Represents an address.

```csharp
public interface IMapAddress
```

## Supported platforms

| Platform | Version |
| --- | --- |
| .NET Standard | 2.0 |
| Xamarin.Android | 9.0 |
| Xamarin.iOS  | 1.0 |
| UWP | 10.0.16299 | 

## Properties

### BuildingName

Gets the building name of an address.

```csharp
string BuildingName { get; }
```

### BuildingFloor

Gets the building floor of an address.

```csharp
string BuildingFloor { get; }
```

### BuildingRoom

Gets the building room of an address.

```csharp
string BuildingRoom { get; }
```

### BuildingWing

Gets the building wing of an address.

```csharp
string BuildingWing { get; }
```

### StreetNumber

Gets the street number of an address.

```csharp
string StreetNumber { get; }
```

### Street

Gets the street name of an address.

```csharp
string Street { get; }
```

### Neighborhood

Gets the neighborhood of an address.

```csharp
string Neighborhood { get; }
```

### District

Gets the district of an address.

```csharp
string District { get; }
```

### Town

Gets the town or city of an address.

```csharp
string Town { get; }
```

### Region

Gets the region (for example, the state or province) of an address.

```csharp
string Region { get; }
```

### RegionCode

Gets the code for the region (for example, the state or province) of an address.

```csharp
string RegionCode { get; }
```

### Country

Gets the country of an address.

```csharp
string Country { get; }
```

### CountryCode

Gets the country code of an address.

```csharp
string CountryCode { get; }
```

### PostCode

Gets the postal code of an address.

```csharp
string PostCode { get; }
```

### Continent

Gets the continent of an address.

```csharp
string Continent { get; }
```