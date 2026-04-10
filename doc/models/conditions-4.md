
# Conditions 4

*This model accepts additional fields of type array.*

## Structure

`Conditions4`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `method` | [`?string(Method5)`](../../doc/models/method-5.md) | Optional | - | getMethod(): ?string | setMethod(?string method): void |
| `values` | [`?string(Values4)`](../../doc/models/values-4.md) | Optional | - | getValues(): ?string | setValues(?string values): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "method": "oxor",
  "values": "token_api_id",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

