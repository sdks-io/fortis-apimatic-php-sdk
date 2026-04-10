
# Joi

*This model accepts additional fields of type array.*

## Structure

`Joi`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `conditions` | [`?Conditions`](../../doc/models/conditions.md) | Optional | - | getConditions(): ?Conditions | setConditions(?Conditions conditions): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "account_vault_api_id",
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

