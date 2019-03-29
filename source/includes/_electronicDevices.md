# Electronic Devices

## Create new electronic device
```shell

```

```javascript

```

```csharp

SpaceElectronicDeviceCreateOptions createOptions = new SpaceElectronicDeviceCreateOptions
{
    BusinessPremiseId = "BUSINESS_PREMISE_ID",
    ElectronicDeviceId = "ELECTRONIC_DEVICE_ID",
    Environment = "test",
    OrganizationId = "ORGANIZATION_ID"
};

SpaceElectronicDeviceService electronicDeviceService = new SpaceElectronicDeviceService();
SpaceElectronicDevice electronicDevice = electronicDeviceService.Create("BUSINESS_PREMISE_ID", createOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceElectronicDevice
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("electronicDeviceId")]
    public string ElectronicDeviceId { get; set; }

    [JsonProperty("numbers")]
    public List<SpaceNumber> Numbers { get; set; }

    [JsonProperty("environment")]
    public string Environment { get; set; }

    [JsonProperty("createdAt")]
    public DateTime CreatedAt { get; set; }

    [JsonProperty("businessPremiseId")]
    public string BusinessPremiseId { get; set; }

    [JsonProperty("organizationId")]
    public string OrganizationId { get; set; }

}
```

```php

```

## List electronic devices
```shell

```

```javascript

```

```csharp

SpaceElectronicDeviceService electronicDeviceService = new SpaceElectronicDeviceService();
List<SpaceElectronicDevice> devices = electronicDeviceService.List("ORGANIZATION_ID");
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
List<paceElectronicDevice>
```

```php

```

## Patch attributes
```shell

```

```javascript

```

```csharp

SpaceEectronicDevicePatchOptions patchOptions = new SpaceEectronicDevicePatchOptions
{
    BusinessPremiseId = "BUSINESS_PREMISE_ID",
    ElectronicDeviceId = "ELECTRONIC_DEVICE_ID",
    Environment = "test",
    OrganizationId = "ORGANIZATION_ID"
};

SpaceElectronicDeviceService electronicDeviceService = new SpaceElectronicDeviceService();
List<SpaceElectronicDevice> devices = electronicDeviceService.PatchAttributes("ELECTRONIC_DEVICE_ID", patchOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceElectronicDevice
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("electronicDeviceId")]
    public string ElectronicDeviceId { get; set; }

    [JsonProperty("numbers")]
    public List<SpaceNumber> Numbers { get; set; }

    [JsonProperty("environment")]
    public string Environment { get; set; }

    [JsonProperty("createdAt")]
    public DateTime CreatedAt { get; set; }

    [JsonProperty("businessPremiseId")]
    public string BusinessPremiseId { get; set; }

    [JsonProperty("organizationId")]
    public string OrganizationId { get; set; }

}
```

```php

```