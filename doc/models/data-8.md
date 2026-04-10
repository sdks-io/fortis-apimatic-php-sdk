
# Data 8

*This model accepts additional fields of type array.*

## Structure

`Data8`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `action` | `?array` | Optional | - | getAction(): ?array | setAction(?array action): void |
| `digitalWalletsOnly` | `?bool` | Optional | **Default**: `false` | getDigitalWalletsOnly(): ?bool | setDigitalWalletsOnly(?bool digitalWalletsOnly): void |
| `methods` | [`?(Method3[])`](../../doc/models/method-3.md) | Optional | By default the system will try to offer all the availables payment methods from your account. However, if you need to display only cc or ach only use the corresponding product transaction id.<br><br>**Constraints**: *Minimum Items*: `1`, *Unique Items Required* | getMethods(): ?array | setMethods(?array methods): void |
| `amount` | `?int` | Optional | The total transaction amount to be charged with the transaction intention. Allowed on the actions: `sale`, `auth-only`, `refund`<br><br>**Constraints**: `>= 1`, `<= 999999999` | getAmount(): ?int | setAmount(?int amount): void |
| `taxAmount` | `?int` | Optional | Amount of Sales Tax. If supplied, this amount should be already included in the transaction amount. Allowed on the actions: `sale`, `auth-only`, `refund`<br><br>**Constraints**: `>= 1`, `<= 999999999` | getTaxAmount(): ?int | setTaxAmount(?int taxAmount): void |
| `secondaryAmount` | `?int` | Optional | secondary_amount is used as a mechanism for partners to collect platform or SaAs fees at a transaction level. This field is intended for use with ISV integrations not standalone merchant integrations. Allowed on the actions: `sale`, `auth-only`.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getSecondaryAmount(): ?int | setSecondaryAmount(?int secondaryAmount): void |
| `locationId` | `?string` | Optional | Location ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getLocationId(): ?string | setLocationId(?string locationId): void |
| `contactId` | `?string` | Optional | Contact ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getContactId(): ?string | setContactId(?string contactId): void |
| `saveAccount` | `?bool` | Optional | Specifies to tokenize card/bank information within the transaction. Allowed on the actions: `sale`, `auth-only`, `avs-only`, `refund`. Do not include with `tokeniation` action. | getSaveAccount(): ?bool | setSaveAccount(?bool saveAccount): void |
| `saveAccountTitle` | `?string` | Optional | Specifies to tokenize card/bank information within the transaction. Allowed on the actions: `sale`, `auth-only`, `avs-only`, `refund`. Do not include with `tokeniation` action.<br><br>**Constraints**: *Maximum Length*: `16` | getSaveAccountTitle(): ?string | setSaveAccountTitle(?string saveAccountTitle): void |
| `title` | `?string` | Optional | A title for the token.<br><br>**Constraints**: *Maximum Length*: `16` | getTitle(): ?string | setTitle(?string title): void |
| `achSecCode` | `?array` | Optional | - | getAchSecCode(): ?array | setAchSecCode(?array achSecCode): void |
| `bankFundedOnlyOverride` | `?bool` | Optional | Bank Funded Only Override. Force the use of a bank funded debit card on debit repayment type transactions. | getBankFundedOnlyOverride(): ?bool | setBankFundedOnlyOverride(?bool bankFundedOnlyOverride): void |
| `allowPartialAuthorizationOverride` | `?bool` | Optional | Allow partial Authorization Override. Must have Fortis approval for production access. | getAllowPartialAuthorizationOverride(): ?bool | setAllowPartialAuthorizationOverride(?bool allowPartialAuthorizationOverride): void |
| `autoDeclineCvvOverride` | `?bool` | Optional | Auto Decline Cvv Override | getAutoDeclineCvvOverride(): ?bool | setAutoDeclineCvvOverride(?bool autoDeclineCvvOverride): void |
| `autoDeclineStreetOverride` | `?bool` | Optional | Auto Decline Street Override | getAutoDeclineStreetOverride(): ?bool | setAutoDeclineStreetOverride(?bool autoDeclineStreetOverride): void |
| `autoDeclineZipOverride` | `?bool` | Optional | Auto Decline Zip Override | getAutoDeclineZipOverride(): ?bool | setAutoDeclineZipOverride(?bool autoDeclineZipOverride): void |
| `message` | `?string` | Optional | A custom text message that displays after the payment is processed.<br><br>**Constraints**: *Maximum Length*: `120` | getMessage(): ?string | setMessage(?string message): void |
| `clientToken` | `?string` | Optional | A JWT to be used to create the elements.<br><br>> This is a one-time only use token.<br>> Do not store for long term use. | getClientToken(): ?string | setClientToken(?string clientToken): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "digitalWalletsOnly": false,
  "amount": 1099,
  "location_id": "11e95f8ec39de8fbdb0a4f1a",
  "contact_id": "11e95f8ec39de8fbdb0a4f1a",
  "client_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c",
  "action": {
    "key1": "val1",
    "key2": "val2"
  },
  "methods": [
    {
      "type": "ach",
      "product_transaction_id": "product_transaction_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "ach",
      "product_transaction_id": "product_transaction_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "ach",
      "product_transaction_id": "product_transaction_id4",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "tax_amount": 94,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

