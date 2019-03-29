# Access Tokens

## Create new access token
```shell

```

```javascript

```

```csharp
SpaceAccessTokenCreateOptions createOptions = new SpaceAccessTokenCreateOptions
{
    Ttl = -1
};

SpaceAccessTokenService spaceAccessTokenService = new SpaceAccessTokenService();
SpaceAccessToken accessToken = spaceAccessTokenService.Create("USER_ID", createOptions);
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
public class SpaceAccessToken
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("ttl")]
    public int Ttl { get; set; }

    [JsonProperty("scopes")]
    public List<string> Scopes { get; set; }

    [JsonProperty("created")]
    public DateTime Created { get; set; }

    [JsonProperty("userId")]
    public string UserId { get; set; }

}
```

```php

```

## List access tokens
```shell

```

```javascript

```

```csharp
SpaceAccessTokenService spaceAccessTokenService = new SpaceAccessTokenService();
List<SpaceAccessToken> accessToken = spaceAccessTokenService.List("USER_ID");
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
List<SpaceAccessToken>

public class SpaceAccessToken
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("ttl")]
    public int Ttl { get; set; }

    [JsonProperty("scopes")]
    public List<string> Scopes { get; set; }

    [JsonProperty("created")]
    public DateTime Created { get; set; }

    [JsonProperty("userId")]
    public string UserId { get; set; }

}
```

```php

```

## Delete access token
```shell

```

```javascript

```

```csharp
SpaceAccessTokenService spaceAccessTokenService = new SpaceAccessTokenService();
SpaceResponse delete = spaceAccessTokenService.Delete("USER_D", "ACCESS_TOKEN_ID");
```

```php

```


> Returns:

```shell
```

```javascript
```

```csharp
List<SpaceAccessToken>

public class SpaceAccessToken
{
    [JsonProperty("id")]
    public string Id { get; set; }

    [JsonProperty("ttl")]
    public int Ttl { get; set; }

    [JsonProperty("scopes")]
    public List<string> Scopes { get; set; }

    [JsonProperty("created")]
    public DateTime Created { get; set; }

    [JsonProperty("userId")]
    public string UserId { get; set; }

}
```

```php

```