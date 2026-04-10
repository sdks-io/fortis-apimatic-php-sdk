
# Response Device Term

*This model accepts additional fields of type array.*

## Structure

`ResponseDeviceTerm`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type22)`](../../doc/models/type-22.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data6`](../../doc/models/data-6.md) | Optional | - | getData(): ?Data6 | setData(?Data6 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "DeviceTerm",
  "data": {
    "location_id": "location_id4",
    "terminal_id": "terminal_id6",
    "require_signature": false,
    "device_term_api_id": "device_term_api_id0",
    "terms_conditions": "terms_conditions0",
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

