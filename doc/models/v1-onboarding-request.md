
# V1 Onboarding Request

*This model accepts additional fields of type array.*

## Structure

`V1OnboardingRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `parentId` | `?string` | Optional | Location ID | getParentId(): ?string | setParentId(?string parentId): void |
| `primaryPrincipal` | [`PrimaryPrincipal2`](../../doc/models/primary-principal-2.md) | Required | - | getPrimaryPrincipal(): PrimaryPrincipal2 | setPrimaryPrincipal(PrimaryPrincipal2 primaryPrincipal): void |
| `templateCode` | `string` | Required | The ID of the template to be used - this value will be provided by Fortis.<br><br>**Constraints**: *Maximum Length*: `20`, *Pattern*: `^[a-zA-Z0-9]*$` | getTemplateCode(): string | setTemplateCode(string templateCode): void |
| `email` | `string` | Required | Merchant email address.<br><br>**Constraints**: *Maximum Length*: `100` | getEmail(): string | setEmail(string email): void |
| `dbaName` | `string` | Required | Merchant 'Doing Business As' name.<br><br>**Constraints**: *Maximum Length*: `100` | getDbaName(): string | setDbaName(string dbaName): void |
| `location` | [`Location19`](../../doc/models/location-19.md) | Required | - | getLocation(): Location19 | setLocation(Location19 location): void |
| `appDelivery` | [`string(AppDelivery)`](../../doc/models/app-delivery.md) | Required | **Constraints**: *Maximum Length*: `12` | getAppDelivery(): string | setAppDelivery(string appDelivery): void |
| `businessCategory` | `?array` | Optional | - | getBusinessCategory(): ?array | setBusinessCategory(?array businessCategory): void |
| `businessType` | `?array` | Optional | - | getBusinessType(): ?array | setBusinessType(?array businessType): void |
| `businessDescription` | `?string` | Optional | Description of Goods or Services.<br><br>**Constraints**: *Maximum Length*: `200` | getBusinessDescription(): ?string | setBusinessDescription(?string businessDescription): void |
| `swipedPercent` | `?int` | Optional | Card present/swiped percentage<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | getSwipedPercent(): ?int | setSwipedPercent(?int swipedPercent): void |
| `keyedPercent` | `?int` | Optional | Card not present/keyed percentage<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | getKeyedPercent(): ?int | setKeyedPercent(?int keyedPercent): void |
| `ecommercePercent` | `?int` | Optional | eCommerce percentage.<br><br>> The sum total of "swiped_percent", "keyed_percent" and "ecommerce_percent" must add up to 100.<br><br>**Constraints**: `>= 0`, `<= 100` | getEcommercePercent(): ?int | setEcommercePercent(?int ecommercePercent): void |
| `ownershipType` | `?array` | Optional | - | getOwnershipType(): ?array | setOwnershipType(?array ownershipType): void |
| `fedTaxId` | `?string` | Optional | Federal Tax ID (EIN).<br><br>**Constraints**: *Maximum Length*: `10` | getFedTaxId(): ?string | setFedTaxId(?string fedTaxId): void |
| `ccAverageTicketRange` | `?int` | Optional | Average Transaction Amount Range<br><br>> (Applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | getCcAverageTicketRange(): ?int | setCcAverageTicketRange(?int ccAverageTicketRange): void |
| `ccMonthlyVolumeRange` | `?int` | Optional | Monthly Processing Volume Range<br><br>> (Applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | getCcMonthlyVolumeRange(): ?int | setCcMonthlyVolumeRange(?int ccMonthlyVolumeRange): void |
| `ccHighTicket` | `?int` | Optional | Highest transaction amount rounded to the next dollar<br><br>> (No decimal and applicable when Template Application Type is 'credit_card' or 'both').<br><br>**Constraints**: `>= 0`, `<= 30000` | getCcHighTicket(): ?int | setCcHighTicket(?int ccHighTicket): void |
| `ecAverageTicketRange` | `?int` | Optional | Average Transaction Amount Range<br><br>> (Applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | getEcAverageTicketRange(): ?int | setEcAverageTicketRange(?int ecAverageTicketRange): void |
| `ecMonthlyVolumeRange` | `?int` | Optional | Monthly Processing Volume Range<br><br>> (Applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 1`, `<= 7` | getEcMonthlyVolumeRange(): ?int | setEcMonthlyVolumeRange(?int ecMonthlyVolumeRange): void |
| `ecHighTicket` | `?int` | Optional | Highest transaction amount rounded to the next dollar<br><br>> (No decimal and applicable when Template Application Type is 'echeck' or 'both').<br><br>**Constraints**: `>= 0`, `<= 30000` | getEcHighTicket(): ?int | setEcHighTicket(?int ecHighTicket): void |
| `website` | `?string` | Optional | Merchant's business website.<br><br>> (Required if "ecommerce_percent" is greater than 0).<br><br>**Constraints**: *Maximum Length*: `100` | getWebsite(): ?string | setWebsite(?string website): void |
| `bankAccount` | [`?BankAccount3`](../../doc/models/bank-account-3.md) | Optional | - | getBankAccount(): ?BankAccount3 | setBankAccount(?BankAccount3 bankAccount): void |
| `altBankAccount` | [`?AltBankAccount2`](../../doc/models/alt-bank-account-2.md) | Optional | - | getAltBankAccount(): ?AltBankAccount2 | setAltBankAccount(?AltBankAccount2 altBankAccount): void |
| `legalName` | `?string` | Optional | Merchant legal name.<br><br>> (leave blank if same as DBA name).<br><br>**Constraints**: *Maximum Length*: `100` | getLegalName(): ?string | setLegalName(?string legalName): void |
| `contact` | [`Contact13`](../../doc/models/contact-13.md) | Required | - | getContact(): Contact13 | setContact(Contact13 contact): void |
| `clientAppId` | `?string` | Optional | Client Issues Id to track that can be used to track each submitted merchant application. This id should be generated and sent in the request payload, and will be returned in the response payload. If no id is submitted in the payload request, this field will be null in the response.<br><br>**Constraints**: *Maximum Length*: `50` | getClientAppId(): ?string | setClientAppId(?string clientAppId): void |
| `secCodes` | [`?(string(SecCode)[])`](../../doc/models/sec-code.md) | Optional | Array of SEC codes that will be allowed, Only applicable for ACH. Valid values are 'PPD', 'WEB', 'TEL', 'CCD'. | getSecCodes(): ?array | setSecCodes(?array secCodes): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "primary_principal": {
    "first_name": "Bob",
    "last_name": "Fairview",
    "middle_name": "Nathaniel",
    "title": "Dr",
    "date_of_birth": "2021-12-01",
    "address_line_1": "1354 Oak St.",
    "address_line_2": "Unit 203",
    "city": "Dover",
    "state_province": "DE",
    "postal_code": "55022",
    "ownership_percent": 100,
    "phone_number": "555-555-1234",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "template_code": "1234YourTemplateCode",
  "email": "email@domain.com",
  "dba_name": "Discount Home Goods",
  "location": {
    "address_line_1": "1200 West Hartford Pkwy",
    "address_line_2": "Suite 2000",
    "city": "Dover",
    "state_province": "DE",
    "postal_code": "55022",
    "phone_number": "555-555-1212",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "app_delivery": "direct",
  "swiped_percent": 0,
  "keyed_percent": 0,
  "ecommerce_percent": 100,
  "fed_tax_id": "0000000000",
  "cc_average_ticket_range": 5,
  "cc_monthly_volume_range": 1,
  "cc_high_ticket": 1500,
  "ec_average_ticket_range": 5,
  "ec_monthly_volume_range": 2,
  "ec_high_ticket": 1500,
  "website": "http://www.example.com",
  "legal_name": "Total Home Goods, LLP",
  "contact": {
    "first_name": "Jeffery",
    "last_name": "Todd",
    "email": "jtodd@example.com",
    "phone_number": "555-555-3456",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "client_app_id": "ABC123",
  "parent_id": "parent_id8",
  "business_category": {
    "key1": "val1",
    "key2": "val2"
  },
  "business_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "business_description": "business_description0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

