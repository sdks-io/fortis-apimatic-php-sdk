
# Response Remove Verification

*This model accepts additional fields of type array.*

## Structure

`ResponseRemoveVerification`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type134)`](../../doc/models/type-134.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data32`](../../doc/models/data-32.md) | Optional | - | getData(): ?Data32 | setData(?Data32 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "RemoveVerification",
  "data": {
    "id": "id0",
    "user_id": "user_id8",
    "hash": "hash6",
    "created_ts": 114,
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

