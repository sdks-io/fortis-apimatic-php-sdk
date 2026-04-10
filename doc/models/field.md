
# Field

*This model accepts additional fields of type array.*

## Structure

`Field`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `field` | `?string` | Optional | Field name used on the sort | getField(): ?string | setField(?string field): void |
| `order` | [`?string(Order)`](../../doc/models/order.md) | Optional | - | getOrder(): ?string | setOrder(?string order): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "field": "last_name",
  "order": "asc",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

