
# Response Async Status

*This model accepts additional fields of type array.*

## Structure

`ResponseAsyncStatus`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type)`](../../doc/models/type.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data`](../../doc/models/data.md) | Optional | - | getData(): ?Data | setData(?Data data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "AsyncStatus",
  "data": {
    "code": "00001e1c-0000-0000-0000-000000000000",
    "type": "type0",
    "id": "id0",
    "progress": 100,
    "error": "error4",
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

