
# Response Tag

*This model accepts additional fields of type array.*

## Structure

`ResponseTag`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type77)`](../../doc/models/type-77.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data22`](../../doc/models/data-22.md) | Optional | - | getData(): ?Data22 | setData(?Data22 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "Tag",
  "data": {
    "location_id": "location_id4",
    "title": "title6",
    "id": "id0",
    "created_ts": 114,
    "modified_ts": 190,
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

