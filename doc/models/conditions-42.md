
# Conditions 42

*This model accepts additional fields of type array.*

## Structure

`Conditions42`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `method` | [`?string(Method5)`](../../doc/models/method-5.md) | Optional | - | getMethod(): ?string | setMethod(?string method): void |
| `values` | [`?string(Values6)`](../../doc/models/values-6.md) | Optional | - | getValues(): ?string | setValues(?string values): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "method": "oxor",
  "values": "accountvault_c2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

