
# Reason Code 1

*This model accepts additional fields of type array.*

## Structure

`ReasonCode1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `id` | `?int` | Optional | ID | getId(): ?int | setId(?int id): void |
| `title` | `?string` | Optional | Title | getTitle(): ?string | setTitle(?string title): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "id": 50,
  "title": "Sample Title",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

