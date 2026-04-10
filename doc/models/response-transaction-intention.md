
# Response Transaction Intention

*This model accepts additional fields of type array.*

## Structure

`ResponseTransactionIntention`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type28)`](../../doc/models/type-28.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data8`](../../doc/models/data-8.md) | Optional | - | getData(): ?Data8 | setData(?Data8 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "TransactionIntention",
  "data": {
    "action": {
      "key1": "val1",
      "key2": "val2"
    },
    "digitalWalletsOnly": false,
    "methods": [
      {
        "type": "ach",
        "product_transaction_id": "product_transaction_id4",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
    ],
    "amount": 236,
    "tax_amount": 218,
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

