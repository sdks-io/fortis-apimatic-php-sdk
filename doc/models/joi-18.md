
# Joi 18

*This model accepts additional fields of type array.*

## Structure

`Joi18`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `conditions` | [Conditions18](../../doc/models/conditions-18.md)\|[Conditions18](../../doc/models/conditions-18.md)1\|[Conditions4](../../doc/models/conditions-4.md)\|[Conditions4](../../doc/models/conditions-4.md)1\|[Conditions4](../../doc/models/conditions-4.md)2\|[Conditions4](../../doc/models/conditions-4.md)3\|null | Optional | This is a container for any-of cases. | getConditions(): | setConditions( conditions): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "conditions": {
    "method": "xor",
    "values": "account_number",
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

