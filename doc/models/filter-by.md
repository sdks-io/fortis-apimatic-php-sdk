
# Filter By

*This model accepts additional fields of type array.*

## Structure

`FilterBy`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `key` | `string` | Required | Resource key to filter by | getKey(): string | setKey(string key): void |
| `operator` | string([Operator1](../../doc/models/operator-1.md)) | Required | This is a container for one-of cases. | getOperator(): string | setOperator(string operator): void |
| `value` | float\|string\|bool | Required | This is a container for one-of cases. | getValue(): | setValue( value): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "key": "first_name",
  "operator": "<=",
  "value": "Fred",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

