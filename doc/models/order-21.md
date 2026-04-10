
# Order 21

*This model accepts additional fields of type array.*

## Structure

`Order21`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `key` | `string` | Required | Resource key to order by. | getKey(): string | setKey(string key): void |
| `operator` | [`string(Operator)`](../../doc/models/operator.md) | Required | - | getOperator(): string | setOperator(string operator): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "asc",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

