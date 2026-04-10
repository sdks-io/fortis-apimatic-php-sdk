
# Settings

*This model accepts additional fields of type array.*

## Structure

`Settings`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `enabled` | `?bool` | Optional | Enabled | getEnabled(): ?bool | setEnabled(?bool enabled): void |
| `columns` | `?float` | Optional | Columns | getColumns(): ?float | setColumns(?float columns): void |
| `rows` | `?float` | Optional | Rows | getRows(): ?float | setRows(?float rows): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "enabled": true,
  "columns": 1.0,
  "rows": 1.0,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

