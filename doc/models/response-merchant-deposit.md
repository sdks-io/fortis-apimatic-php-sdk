
# Response Merchant Deposit

*This model accepts additional fields of type array.*

## Structure

`ResponseMerchantDeposit`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type47)`](../../doc/models/type-47.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data14`](../../doc/models/data-14.md) | Optional | - | getData(): ?Data14 | setData(?Data14 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "MerchantDeposit",
  "data": {
    "id": "id0",
    "company_id": "company_id6",
    "merchant_id": "merchant_id0",
    "service": "service0",
    "deposit_types": [
      "deposit",
      "adjustment",
      "fee"
    ],
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

