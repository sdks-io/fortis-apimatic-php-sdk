
# Response Three Ds Authentication

*This model accepts additional fields of type array.*

## Structure

`ResponseThreeDsAuthentication`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type45)`](../../doc/models/type-45.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data12`](../../doc/models/data-12.md) | Optional | - | getData(): ?Data12 | setData(?Data12 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "ThreeDSAuthentication",
  "data": {
    "three_ds_server_trans_id": "three_ds_server_trans_id0",
    "acs_url": "acs_url2",
    "transaction_status": "D",
    "authentication_value": "authentication_value2",
    "eci": "eci0",
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

