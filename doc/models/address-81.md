
# Address 81

Array of merchant addresses.

*This model accepts additional fields of type array.*

## Structure

`Address81`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `addressLine1` | `string` | Required | Line 1 of address.<br><br>**Constraints**: *Maximum Length*: `100` | getAddressLine1(): string | setAddressLine1(string addressLine1): void |
| `addressLine2` | `?string` | Optional | Line 2 of address.<br><br>**Constraints**: *Maximum Length*: `20` | getAddressLine2(): ?string | setAddressLine2(?string addressLine2): void |
| `city` | `string` | Required | City of address.<br><br>**Constraints**: *Maximum Length*: `50` | getCity(): string | setCity(string city): void |
| `stateProvince` | `string` | Required | State or province of address.<br><br>**Constraints**: *Maximum Length*: `2` | getStateProvince(): string | setStateProvince(string stateProvince): void |
| `postalCode` | `string` | Required | Postal code of address.<br><br>**Constraints**: *Maximum Length*: `10` | getPostalCode(): string | setPostalCode(string postalCode): void |
| `countryCode` | `string` | Required | Country of address.<br><br>**Constraints**: *Maximum Length*: `2` | getCountryCode(): string | setCountryCode(string countryCode): void |
| `addressType` | [`string(AddressType)`](../../doc/models/address-type.md) | Required | **Constraints**: *Maximum Length*: `20` | getAddressType(): string | setAddressType(string addressType): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "address_line_1": "121 E Main",
  "address_line_2": "Apt 707",
  "city": "Dallas",
  "state_province": "TX",
  "postal_code": "75087",
  "country_code": "US",
  "address_type": "corporate",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

