
# Conditions 41

*This model accepts additional fields of type array.*

## Structure

`Conditions41`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `method` | [`?string(Method5)`](../../doc/models/method-5.md) | Optional | - | getMethod(): ?string | setMethod(?string method): void |
| `values` | [`?string(Values5)`](../../doc/models/values-5.md) | Optional | - | getValues(): ?string | setValues(?string values): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "method": "oxor",
  "values": "accountvault_c1",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

