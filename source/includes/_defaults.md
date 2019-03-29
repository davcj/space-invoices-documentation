# Defaults

## Create default
```shell

```

```javascript

```

```csharp
SpaceDefaultCreateOptions createOptions = new SpaceDefaultCreateOptions
{
    Name = "new default",
    Value = "new default value"
};

SpaceDefaultService defaultService = new SpaceDefaultService();
SpaceDefault default = defaultService.Create("ORGANIZATION_ID", createOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceDefault
{
  [JsonProperty("id")]
  public string Id { get; set; }

  [JsonProperty("name")]
  public string Name { get; set; }

  [JsonProperty("value")]
  public string Value { get; set; }

}
```

```php

```

## Update default
```shell

```

```javascript

```

```csharp


SpaceDefaultUpdateOptions updateOptions = new SpaceDefaultUpdateOptions
{
  Value = "new default value"
};

SpaceDefaultService defaultService = new SpaceDefaultService();
SpaceDefault default = defaultService.Update("ORGANIZATION_ID", "DEFAULT_ID", updateOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceDefault
{
  [JsonProperty("id")]
  public string Id { get; set; }

  [JsonProperty("name")]
  public string Name { get; set; }

  [JsonProperty("value")]
  public string Value { get; set; }

}
```

```php

```

## List defaults
```shell

```

```javascript

```

```csharp
SpaceDefaultService defaultService = new SpaceDefaultService();
List<SpaceDefault> defaults = defaultService.List("ORGANIZATION_ID");
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
List<SpaceDefault>

public class SpaceDefault
{
  [JsonProperty("id")]
  public string Id { get; set; }

  [JsonProperty("name")]
  public string Name { get; set; }

  [JsonProperty("value")]
  public string Value { get; set; }

}
```

```php

```

