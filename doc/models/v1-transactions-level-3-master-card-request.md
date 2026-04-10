
# V1 Transactions Level 3 Master Card Request

*This model accepts additional fields of type array.*

## Structure

`V1TransactionsLevel3MasterCardRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `level3Data` | [`Level3Data3`](../../doc/models/level-3-data-3.md) | Required | - | getLevel3Data(): Level3Data3 | setLevel3Data(Level3Data3 level3Data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "level3_data": {
    "destination_country_code": "840",
    "duty_amount": 0,
    "freight_amount": 0,
    "national_tax": 2,
    "sales_tax": 200,
    "shipfrom_zip_code": "AZ12345",
    "shipto_zip_code": "MI48335",
    "tax_amount": 0,
    "line_items": [
      {
        "alternate_tax_id": "1234",
        "description": "cool drink",
        "discount_amount": 10,
        "discount_rate": 11,
        "product_code": "coke12345678",
        "quantity": 5,
        "tax_amount": 3,
        "tax_rate": 0,
        "tax_type_applied": "22",
        "tax_type_id": "a1",
        "unit_code": "gll",
        "unit_cost": 10,
        "debit_credit": {
          "key1": "val1",
          "key2": "val2"
        },
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
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

