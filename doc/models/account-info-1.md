
# Account Info 1

*This model accepts additional fields of type array.*

## Structure

`AccountInfo1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `chAccAgeInd` | [`?string(ChAccAgeInd)`](../../doc/models/ch-acc-age-ind.md) | Optional | - | getChAccAgeInd(): ?string | setChAccAgeInd(?string chAccAgeInd): void |
| `chAccDate` | `?string` | Optional | Date converted into UTC that the cardholder opened the account with the 3DS Requestor. Date format = YYYYMMDD. | getChAccDate(): ?string | setChAccDate(?string chAccDate): void |
| `chAccChangeInd` | [`?string(ChAccChangeInd)`](../../doc/models/ch-acc-change-ind.md) | Optional | - | getChAccChangeInd(): ?string | setChAccChangeInd(?string chAccChangeInd): void |
| `chAccChange` | `?string` | Optional | Date converted into UTC that the cardholder's account with the 3DS Requestor was last changed. Including Billing or Shipping address, new payment account, or new user(s) added. Date format = YYYYMMDD. | getChAccChange(): ?string | setChAccChange(?string chAccChange): void |
| `chAccPwChangeInd` | [`?string(ChAccPwChangeInd)`](../../doc/models/ch-acc-pw-change-ind.md) | Optional | - | getChAccPwChangeInd(): ?string | setChAccPwChangeInd(?string chAccPwChangeInd): void |
| `chAccPwChange` | `?string` | Optional | Date converted into UTC that cardholder's account with the 3DS Requestor had a password change or account reset. Date format must be YYYYMMDD. | getChAccPwChange(): ?string | setChAccPwChange(?string chAccPwChange): void |
| `shipAddressUsageInd` | [`?string(ShipAddressUsageInd)`](../../doc/models/ship-address-usage-ind.md) | Optional | - | getShipAddressUsageInd(): ?string | setShipAddressUsageInd(?string shipAddressUsageInd): void |
| `shipAddressUsage` | `?string` | Optional | Date converted into UTC when the shipping address used for this transaction was first used with the 3DS Requestor. Date format must be YYYYMMDD. | getShipAddressUsage(): ?string | setShipAddressUsage(?string shipAddressUsage): void |
| `txnActivityDay` | `?int` | Optional | Number of transactions (successful and abandoned) for this cardholder account with the 3DS Requestor across all payment accounts in the previous 24 hours. | getTxnActivityDay(): ?int | setTxnActivityDay(?int txnActivityDay): void |
| `txnActivityYear` | `?int` | Optional | Number of transactions (successful and abandoned) for this cardholder account with the 3DS Requestor across all payment accounts in the previous year. | getTxnActivityYear(): ?int | setTxnActivityYear(?int txnActivityYear): void |
| `provisionAttemptsDay` | `?int` | Optional | Number of Add Card attempts in the last 24 hours. | getProvisionAttemptsDay(): ?int | setProvisionAttemptsDay(?int provisionAttemptsDay): void |
| `nbPurchaseAccount` | `?int` | Optional | Number of purchases with this cardholder account during the previous six months. | getNbPurchaseAccount(): ?int | setNbPurchaseAccount(?int nbPurchaseAccount): void |
| `suspiciousAccActivity` | [`?string(SuspiciousAccActivity)`](../../doc/models/suspicious-acc-activity.md) | Optional | - | getSuspiciousAccActivity(): ?string | setSuspiciousAccActivity(?string suspiciousAccActivity): void |
| `shipNameIndicator` | [`?string(ShipNameIndicator)`](../../doc/models/ship-name-indicator.md) | Optional | - | getShipNameIndicator(): ?string | setShipNameIndicator(?string shipNameIndicator): void |
| `paymentAccInd` | [`?string(PaymentAccInd)`](../../doc/models/payment-acc-ind.md) | Optional | - | getPaymentAccInd(): ?string | setPaymentAccInd(?string paymentAccInd): void |
| `paymentAccAge` | `?string` | Optional | Date converted into UTC that the payment account was enrolled in the cardholder's account with the 3DS Requestor. Date format must be YYYYMMDD. | getPaymentAccAge(): ?string | setPaymentAccAge(?string paymentAccAge): void |
| `chAccReqId` | `?string` | Optional | The 3DS Requestor assigned account identifier of the transacting Cardholder. This identifier is a unique representation of the account identifier for the 3DS Requestor and is provided as a String.<br><br>This field is supported in Starting from EMV 3DS 2.3.1 and later.<br><br>**Constraints**: *Maximum Length*: `64` | getChAccReqId(): ?string | setChAccReqId(?string chAccReqId): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "ch_acc_date": "20240401",
  "ch_acc_change": "20240401",
  "ch_acc_pw_change": "20240401",
  "ship_address_usage": "20240401",
  "txn_activity_day": 1,
  "txn_activity_year": 1,
  "provision_attempts_day": 1,
  "nb_purchase_account": 1,
  "payment_acc_age": "20240401",
  "ch_acc_age_ind": "01",
  "ch_acc_change_ind": "03",
  "ch_acc_pw_change_ind": "04",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

