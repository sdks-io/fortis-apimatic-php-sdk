
# Cardholder Account

Contains information for the Cardholder Account.

*This model accepts additional fields of type array.*

## Structure

`CardholderAccount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `expireDate` | `?string` | Optional | Expiry date of the PAN or token supplied to the 3DS Requestor by the Cardholder. The field has 4 characters in a format YYMM.<br>The requirements of the presence of this field are DS specific. | getExpireDate(): ?string | setExpireDate(?string expireDate): void |
| `accountInfo` | [`?AccountInfo1`](../../doc/models/account-info-1.md) | Optional | - | getAccountInfo(): ?AccountInfo1 | setAccountInfo(?AccountInfo1 accountInfo): void |
| `accountNumber` | `string` | Required | Account number that will be used in the authorization request for payment transactions. May be represented by PAN or token. | getAccountNumber(): string | setAccountNumber(string accountNumber): void |
| `schemeId` | [`string(SchemeId)`](../../doc/models/scheme-id.md) | Required | - | getSchemeId(): string | setSchemeId(string schemeId): void |
| `accountId` | `?string` | Optional | Additional information about the account optionally provided by the 3DS Requestor. | getAccountId(): ?string | setAccountId(?string accountId): void |
| `cvv` | `?string` | Optional | Three or four-digit security code printed on the card. This field is required depending on the rules provided by the Directory Server. Available for supporting EMV 3DS 2.3.1 and later versions.<br><br>**Constraints**: *Minimum Length*: `3`, *Maximum Length*: `4` | getCvv(): ?string | setCvv(?string cvv): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "expire_date": "2508",
  "account_number": "5454545454545454",
  "scheme_id": "Visa",
  "account_info": {
    "ch_acc_age_ind": "02",
    "ch_acc_date": "ch_acc_date4",
    "ch_acc_change_ind": "03",
    "ch_acc_change": "ch_acc_change2",
    "ch_acc_pw_change_ind": "02",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "account_id": "account_id8",
  "cvv": "cvv4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

