
# Line Item

*This model accepts additional fields of type array.*

## Structure

`LineItem`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `alternateTaxId` | `?string` | Optional | Tax identification number of the merchant that reported the alternate tax amount.<br><br>**Constraints**: *Minimum Length*: `1`, *Maximum Length*: `15` | getAlternateTaxId(): ?string | setAlternateTaxId(?string alternateTaxId): void |
| `debitCredit` | `?array` | Optional | - | getDebitCredit(): ?array | setDebitCredit(?array debitCredit): void |
| `description` | `?string` | Optional | Description of the item.<br><br>**Constraints**: *Maximum Length*: `26` | getDescription(): ?string | setDescription(?string description): void |
| `discountAmount` | `?int` | Optional | Total discount amount applied against the line item total ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 99999999999900` | getDiscountAmount(): ?int | setDiscountAmount(?int discountAmount): void |
| `discountRate` | `?int` | Optional | Discount rate for the line item ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 9999900` | getDiscountRate(): ?int | setDiscountRate(?int discountRate): void |
| `productCode` | `?string` | Optional | Merchant-defined description code of the item.<br><br>**Constraints**: *Maximum Length*: `12` | getProductCode(): ?string | setProductCode(?string productCode): void |
| `quantity` | `?int` | Optional | Quantity of the item, can accept Four (4) decimal places.<br><br>**Constraints**: `<= 99999` | getQuantity(): ?int | setQuantity(?int quantity): void |
| `taxAmount` | `?int` | Optional | Amount of any value added taxes, can accept Two (2) decimal places.<br><br>**Constraints**: `>= 0`, `<= 99999999999` | getTaxAmount(): ?int | setTaxAmount(?int taxAmount): void |
| `taxRate` | `?int` | Optional | Tax rate used to calculate the sales tax amount, can accept 2 decimal places.<br><br>**Constraints**: `<= 999900` | getTaxRate(): ?int | setTaxRate(?int taxRate): void |
| `taxTypeApplied` | `?string` | Optional | Type of value-added taxes that are being used (Conditional If tax amount is supplied)<br><br>> This field is only required when Merchant is directed to include by Mastercard.<br><br>**Constraints**: *Maximum Length*: `4` | getTaxTypeApplied(): ?string | setTaxTypeApplied(?string taxTypeApplied): void |
| `taxTypeId` | `?string` | Optional | Indicates the type of tax collected in relationship to a specific tax amount (Conditional If tax amount is supplied)<br><br>**Constraints**: *Maximum Length*: `2` | getTaxTypeId(): ?string | setTaxTypeId(?string taxTypeId): void |
| `unitCode` | `?string` | Optional | Units of measurement as used in international trade. (See Codes for Units of Measurement below for unit code abbreviations)<br><br>**Constraints**: *Maximum Length*: `3` | getUnitCode(): ?string | setUnitCode(?string unitCode): void |
| `unitCost` | `?int` | Optional | Unit cost of the item ,Can accept Four (4) decimal places.<br><br>**Constraints**: `<= 99999999999900` | getUnitCost(): ?int | setUnitCost(?int unitCost): void |
| `commodityCode` | `?string` | Optional | An international description code of the individual good or service being supplied.<br><br>**Constraints**: *Maximum Length*: `12` | getCommodityCode(): ?string | setCommodityCode(?string commodityCode): void |
| `otherTaxAmount` | `?int` | Optional | Used if city or multiple county taxes need to be broken out separately ,Can accept Two (2) decimal places.<br><br>**Constraints**: `<= 99999999999900` | getOtherTaxAmount(): ?int | setOtherTaxAmount(?int otherTaxAmount): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
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
  "commodity_code": "cc123456",
  "other_tax_amount": 0,
  "debit_credit": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

