
# Response Location Info

*This model accepts additional fields of type array.*

## Structure

`ResponseLocationInfo`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type44)`](../../doc/models/type-44.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data11`](../../doc/models/data-11.md) | Optional | - | getData(): ?Data11 | setData(?Data11 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "LocationInfo",
  "data": {
    "id": "id0",
    "created_ts": 114,
    "modified_ts": 190,
    "account_number": "account_number0",
    "address": {
      "city": "city6",
      "state": "state2",
      "postal_code": "postal_code8",
      "country": {
        "key1": "val1",
        "key2": "val2"
      },
      "street": "street6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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

