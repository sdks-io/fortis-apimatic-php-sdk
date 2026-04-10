
# Cardholder

Contains information for the Cardholder. This field is required unless market or regional mandate restricts sending this information.

*This model accepts additional fields of type array.*

## Structure

`Cardholder`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `addressMatch` | [`?string(AddressMatch)`](../../doc/models/address-match.md) | Optional | - | getAddressMatch(): ?string | setAddressMatch(?string addressMatch): void |
| `billingAddress` | [`?BillingAddress13`](../../doc/models/billing-address-13.md) | Optional | - | getBillingAddress(): ?BillingAddress13 | setBillingAddress(?BillingAddress13 billingAddress): void |
| `email` | `?string` | Optional | The email address associated with the account that is either entered by the Cardholder, or is on file with the 3DS Requestor. This field shall meet requirements of Section 3.4 of IETF RFC 5322.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Maximum Length*: `256` | getEmail(): ?string | setEmail(?string email): void |
| `homePhone` | [`?HomePhone2`](../../doc/models/home-phone-2.md) | Optional | - | getHomePhone(): ?HomePhone2 | setHomePhone(?HomePhone2 homePhone): void |
| `mobilePhone` | [`?MobilePhone2`](../../doc/models/mobile-phone-2.md) | Optional | - | getMobilePhone(): ?MobilePhone2 | setMobilePhone(?MobilePhone2 mobilePhone): void |
| `workPhone` | [`?WorkPhone2`](../../doc/models/work-phone-2.md) | Optional | - | getWorkPhone(): ?WorkPhone2 | setWorkPhone(?WorkPhone2 workPhone): void |
| `cardholderName` | `?string` | Optional | Name of the Cardholder.<br><br>This field is required unless market or regional mandate restricts sending this information.<br><br>**Constraints**: *Minimum Length*: `2`, *Maximum Length*: `45` | getCardholderName(): ?string | setCardholderName(?string cardholderName): void |
| `shippingAddress` | [`?ShippingAddress2`](../../doc/models/shipping-address-2.md) | Optional | - | getShippingAddress(): ?ShippingAddress2 | setShippingAddress(?ShippingAddress2 shippingAddress): void |
| `taxId` | `?string` | Optional | Tax ID is the Cardholder's tax identification.<br><br>This field is required depending on the rules provided by the Directory Server.<br>Available for supporting EMV 3DS 2.3.1 and later versions.<br><br>**Constraints**: *Maximum Length*: `45` | getTaxId(): ?string | setTaxId(?string taxId): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "email": "fortis@example.com",
  "cardholder_name": "John Doe",
  "address_match": "Y",
  "billing_address": {
    "city": "city2",
    "country_code": "country_code8",
    "address_line_1": "address_line_12",
    "address_line_2": "address_line_28",
    "address_line_3": "address_line_34",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "home_phone": {
    "cc": "cc8",
    "subscriber": "subscriber0",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "mobile_phone": {
    "cc": "cc8",
    "subscriber": "subscriber0",
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

