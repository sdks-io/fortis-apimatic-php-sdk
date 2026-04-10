
# Multi Transaction 1

*This model accepts additional fields of type array.*

## Structure

`MultiTransaction1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `merchantList` | [`MerchantList[]`](../../doc/models/merchant-list.md) | Required | Contains the details of each merchant involved in the transaction<br><br>**Constraints**: *Minimum Items*: `1`, *Maximum Items*: `50` | getMerchantList(): array | setMerchantList(array merchantList): void |
| `avValidityTime` | `?int` | Optional | Number of days that the AV (Authentication Value) is valid.<br><br>**Constraints**: `>= 0`, `<= 999` | getAvValidityTime(): ?int | setAvValidityTime(?int avValidityTime): void |
| `avNumberUse` | `?int` | Optional | Number of times that the AV (Authentication Value) is valid.<br><br>**Constraints**: `>= 0`, `<= 99` | getAvNumberUse(): ?int | setAvNumberUse(?int avNumberUse): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "merchant_list": [
    {
      "merchant_name_listed": "merchant_name_listed0",
      "acquirer_merchant_id_listed": "acquirer_merchant_id_listed0",
      "merchant_amount": "merchant_amount8",
      "merchant_currency": "merchant_currency6",
      "merchant_exponent": "merchant_exponent0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "av_validity_time": 78,
  "av_number_use": 99,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

