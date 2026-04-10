
# File 5

*This model accepts additional fields of type array.*

## Structure

`File5`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `fileName` | `?string` | Optional | The file name including the extension | getFileName(): ?string | setFileName(?string fileName): void |
| `content` | `?string` | Optional | File contents as a base64 encoded string | getContent(): ?string | setContent(?string content): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "file_name": "file_name6",
  "content": "content6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

