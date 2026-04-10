
# Joi 27

*This model accepts additional fields of type array.*

## Structure

`Joi27`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `conditions` | [`?Conditions27`](../../doc/models/conditions-27.md) | Optional | - | getConditions(): ?Conditions27 | setConditions(?Conditions27 conditions): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "previous_transaction_id",
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

