
# Conditions 18

*This model accepts additional fields of type array.*

## Structure

`Conditions18`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `method` | [`?string(Method)`](../../doc/models/method.md) | Optional | - | getMethod(): ?string | setMethod(?string method): void |
| `values` | [`?string(Values50)`](../../doc/models/values-50.md) | Optional | - | getValues(): ?string | setValues(?string values): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "method": "xor",
  "values": "account_number",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

