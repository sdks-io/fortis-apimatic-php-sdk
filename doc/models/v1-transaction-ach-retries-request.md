
# V1 Transaction Ach Retries Request

*This model accepts additional fields of type array.*

## Structure

`V1TransactionAchRetriesRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `rejectedTransactionId` | `string` | Required | Rejected Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getRejectedTransactionId(): string | setRejectedTransactionId(string rejectedTransactionId): void |
| `returnFee` | `?int` | Optional | Return Fee.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getReturnFee(): ?int | setReturnFee(?int returnFee): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "rejected_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "return_fee": 254,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

