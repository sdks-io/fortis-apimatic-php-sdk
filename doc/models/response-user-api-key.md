
# Response User Api Key

*This model accepts additional fields of type array.*

## Structure

`ResponseUserApiKey`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type128)`](../../doc/models/type-128.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data33`](../../doc/models/data-33.md) | Optional | - | getData(): ?Data33 | setData(?Data33 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "UserApiKey",
  "data": {
    "user_api_key": "user_api_key2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

