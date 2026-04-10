
# Sort

Sort information used on the results

*This model accepts additional fields of type array.*

## Structure

`Sort`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type4)`](../../doc/models/type-4.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `fields` | [`?(Field[])`](../../doc/models/field.md) | Optional | [object Object] | getFields(): ?array | setFields(?array fields): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "Sorting",
  "fields": [
    {
      "field": "field2",
      "order": "asc",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "field": "field2",
      "order": "asc",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

