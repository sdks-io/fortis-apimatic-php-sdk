
# V1 Transactions Level 3 Visa Request

*This model accepts additional fields of type array.*

## Structure

`V1TransactionsLevel3VisaRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `level3Data` | [`Level3Data4`](../../doc/models/level-3-data-4.md) | Required | - | getLevel3Data(): Level3Data4 | setLevel3Data(Level3Data4 level3Data): void |
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
    "shipfrom_zip_code": "AZ1234",
    "shipto_zip_code": "FL1234",
    "tax_amount": 10,
    "customer_vat_registration": "12345678",
    "merchant_vat_registration": "123456",
    "order_date": "171006",
    "summary_commodity_code": "C1K2",
    "tax_rate": 0,
    "unique_vat_ref_number": "vat1234",
    "line_items": [
      {
        "description": "cool drink",
        "commodity_code": "cc123456",
        "discount_amount": 0,
        "other_tax_amount": 0,
        "product_code": "fanta123456",
        "quantity": 12,
        "tax_amount": 4,
        "tax_rate": 0,
        "unit_code": "gll",
        "unit_cost": 3,
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

