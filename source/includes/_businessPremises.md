# Business Premises

## Create new business premise
```shell

```

```javascript

```

```csharp


SpaceBusinessPremiseCreateOptions createOptions = new SpaceBusinessPremiseCreateOptions
{
    BuildingNumber = 5,
    BuildingSectionNumber = 5,
    CadastralNumber = 10,
    City = "Ljubljana",
    Community = "Siska",
    Environment = "test",
    HouseNumber = "5a",
    PostalCode = "1107",
    Street = "Rasiska ulica",
    TaxNumber = "76226719",
    BusinessPremiseID = "BP1",
    Type = "realestate"
};

SpaceBusinessPremiseService businessPremiseService = new SpaceBusinessPremiseService();
SpaceBusinessPremise businessPremise = businessPremiseService.Create("ORGANIZATION_ID", createOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceBusinessPremise
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("type")]
    public string Type { get; set; }

    [JsonProperty("taxNumber")]
    public string TaxNumber { get; set; }

    [JsonProperty("businessPremiseId")]
    public string BusinessPremiseID { get; set; }

    [JsonProperty("premiseType")]
    public string PremiseType { get; set; }

    [JsonProperty("cadastralNumber")]
    public int CadastralNumber { get; set; }

    [JsonProperty("buildingNumber")]
    public int BuildingNumber { get; set; }

    [JsonProperty("buildingSectionNumber")]
    public int BuildingSectionNumber { get; set; }

    [JsonProperty("street")]
    public string Street { get; set; }

    [JsonProperty("houseNumber")]
    public string HouseNumber { get; set; }

    [JsonProperty("houseNumberAdditional")]
    public string HouseNumberAdditional { get; set; }

    [JsonProperty("community")]
    public string Community { get; set; }

    [JsonProperty("city")]
    public string City { get; set; }

    [JsonProperty("postalCode")]
    public string PostalCode { get; set; }

    [JsonProperty("numbers")]
    public List<SpaceNumber> Numbers { get; set; }

    [JsonProperty("environment")]
    public string Environment { get; set; }

    [JsonProperty("createdAt")]
    public DateTime CreatedAt { get; set; }

    [JsonProperty("organizationId")]
    public string OrganizationId { get; set; }

}
```

```php

```

## List business premises
```shell

```

```javascript

```

```csharp


SpaceBusinessPremiseService businessPremiseService = new SpaceBusinessPremiseService();
List<SpaceBusinessPremise> businessPremises = businessPremiseService.List("ORGANIZATION_ID");
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
List<SpaceBusinessPremise>
```

```php

```

## Patch atributes
```shell

```

```javascript

```

```csharp
SpaceBusinessPremisePatchOptions patchOptions = new SpaceBusinessPremisePatchOptions
{
    HouseNumber = "5b",
    PostalCode = "1107",
    Street = "Rasiska ulica",
};


SpaceBusinessPremiseService businessPremiseService = new SpaceBusinessPremiseService();
SpaceBusinessPremise premise = businessPremiseService.PatchAttributes("BUSINESS_PREMISE_ID", patchOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceBusinessPremise
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("type")]
    public string Type { get; set; }

    [JsonProperty("taxNumber")]
    public string TaxNumber { get; set; }

    [JsonProperty("businessPremiseId")]
    public string BusinessPremiseID { get; set; }

    [JsonProperty("premiseType")]
    public string PremiseType { get; set; }

    [JsonProperty("cadastralNumber")]
    public int CadastralNumber { get; set; }

    [JsonProperty("buildingNumber")]
    public int BuildingNumber { get; set; }

    [JsonProperty("buildingSectionNumber")]
    public int BuildingSectionNumber { get; set; }

    [JsonProperty("street")]
    public string Street { get; set; }

    [JsonProperty("houseNumber")]
    public string HouseNumber { get; set; }

    [JsonProperty("houseNumberAdditional")]
    public string HouseNumberAdditional { get; set; }

    [JsonProperty("community")]
    public string Community { get; set; }

    [JsonProperty("city")]
    public string City { get; set; }

    [JsonProperty("postalCode")]
    public string PostalCode { get; set; }

    [JsonProperty("numbers")]
    public List<SpaceNumber> Numbers { get; set; }

    [JsonProperty("environment")]
    public string Environment { get; set; }

    [JsonProperty("createdAt")]
    public DateTime CreatedAt { get; set; }

    [JsonProperty("organizationId")]
    public string OrganizationId { get; set; }

}
```

```php

```
