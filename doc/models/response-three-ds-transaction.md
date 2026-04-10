
# Response Three Ds Transaction

*This model accepts additional fields of type array.*

## Structure

`ResponseThreeDsTransaction`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type46)`](../../doc/models/type-46.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data13`](../../doc/models/data-13.md) | Optional | - | getData(): ?Data13 | setData(?Data13 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "ThreeDSTransaction",
  "data": {
    "three_ds_server_trans_id": "three_ds_server_trans_id0",
    "transaction_status": "transaction_status0",
    "ds_trans_id": "ds_trans_id8",
    "acs_trans_id": "acs_trans_id2",
    "message_version": "message_version0",
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

