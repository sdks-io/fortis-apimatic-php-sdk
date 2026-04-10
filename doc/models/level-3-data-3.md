
# Level 3 Data 3

*This model accepts additional fields of type array.*

## Structure

`Level3Data3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `destinationCountryCode` | `?string` | Optional | Code of the country where the goods are being shipped.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `3` | getDestinationCountryCode(): ?string | setDestinationCountryCode(?string destinationCountryCode): void |
| `dutyAmount` | `?int` | Optional | Fee amount associated with the import of the purchased goods ,Can accept Two (2) decimal places<br><br>**Constraints**: `>= 0`, `<= 99999999999900` | getDutyAmount(): ?int | setDutyAmount(?int dutyAmount): void |
| `freightAmount` | `?int` | Optional | Freight or shipping portion of the total transaction amount ,Can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999900` | getFreightAmount(): ?int | setFreightAmount(?int freightAmount): void |
| `nationalTax` | `?int` | Optional | National tax for the transaction ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 999999999900` | getNationalTax(): ?int | setNationalTax(?int nationalTax): void |
| `salesTax` | `?int` | Optional | Sales tax for the transaction ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 999999999900` | getSalesTax(): ?int | setSalesTax(?int salesTax): void |
| `shipfromZipCode` | `?string` | Optional | Postal/ZIP code of the address from where the purchased goods are being shipped.<br><br>**Constraints**: *Maximum Length*: `10` | getShipfromZipCode(): ?string | setShipfromZipCode(?string shipfromZipCode): void |
| `shiptoZipCode` | `?string` | Optional | Postal/ZIP code of the address where purchased goods will be delivered.<br><br>**Constraints**: *Maximum Length*: `10` | getShiptoZipCode(): ?string | setShiptoZipCode(?string shiptoZipCode): void |
| `taxAmount` | `?int` | Optional | Amount of any value added taxes ,Can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999900` | getTaxAmount(): ?int | setTaxAmount(?int taxAmount): void |
| `taxExempt` | `?array` | Optional | - | getTaxExempt(): ?array | setTaxExempt(?array taxExempt): void |
| `lineItems` | [`LineItem19[]`](../../doc/models/line-item-19.md) | Required | Array of line items in transaction | getLineItems(): array | setLineItems(array lineItems): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
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
}
```

