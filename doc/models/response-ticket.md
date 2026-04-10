
# Response Ticket

*This model accepts additional fields of type array.*

## Structure

`ResponseTicket`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type87)`](../../doc/models/type-87.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data24`](../../doc/models/data-24.md) | Optional | - | getData(): ?Data24 | setData(?Data24 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "Ticket",
  "data": {
    "account_holder_name": "account_holder_name0",
    "exp_date": "exp_date8",
    "cvv": "cvv8",
    "account_number": "account_number0",
    "billing_address": {
      "postal_code": "postal_code0",
      "street": "street8",
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

