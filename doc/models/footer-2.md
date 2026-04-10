
# Footer 2

*This model accepts additional fields of type array.*

## Structure

`Footer2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `settings` | [`?Settings`](../../doc/models/settings.md) | Optional | - | getSettings(): ?Settings | setSettings(?Settings settings): void |
| `fields` | [`?(Field18[])`](../../doc/models/field-18.md) | Optional | - | getFields(): ?array | setFields(?array fields): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "settings": {
    "enabled": false,
    "columns": 202.28,
    "rows": 235.78,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fields": [
    {
      "id": "id8",
      "label": "label8",
      "field_type": "field_type4",
      "position": [
        "position7",
        "position8",
        "position9"
      ],
      "required": false,
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

