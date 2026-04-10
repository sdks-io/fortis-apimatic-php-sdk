
# Conditions 191

*This model accepts additional fields of type array.*

## Structure

`Conditions191`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `method` | [`?string(Method53)`](../../doc/models/method-53.md) | Optional | - | getMethod(): ?string | setMethod(?string method): void |
| `values` | [`?string(Values58)`](../../doc/models/values-58.md) | Optional | - | getValues(): ?string | setValues(?string values): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "method": "and",
  "values": "account_number",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

