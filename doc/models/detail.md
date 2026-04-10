
# Detail

*This model accepts additional fields of type array.*

## Structure

`Detail`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `message` | `?string` | Optional | - | getMessage(): ?string | setMessage(?string message): void |
| `path` | `?(string[])` | Optional | - | getPath(): ?array | setPath(?array path): void |
| `type` | `?string` | Optional | - | getType(): ?string | setType(?string type): void |
| `context` | [`?Context`](../../doc/models/context.md) | Optional | - | getContext(): ?Context | setContext(?Context context): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "message": "\"fieldName\" is required",
  "type": "any.required",
  "path": [
    "path8",
    "path9"
  ],
  "context": {
    "key": "key2",
    "label": "label2",
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

