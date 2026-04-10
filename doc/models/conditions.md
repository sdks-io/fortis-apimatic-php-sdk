
# Conditions

*This model accepts additional fields of type array.*

## Structure

`Conditions`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `method` | [`?string(Method)`](../../doc/models/method.md) | Optional | - | getMethod(): ?string | setMethod(?string method): void |
| `values` | [`?string(Values)`](../../doc/models/values.md) | Optional | - | getValues(): ?string | setValues(?string values): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "method": "xor",
  "values": "account_vault_id",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

