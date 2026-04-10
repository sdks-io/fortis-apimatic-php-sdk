
# Data 26

*This model accepts additional fields of type array.*

## Structure

`Data26`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `rejectedTransactionId` | `?string` | Optional | Rejected Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getRejectedTransactionId(): ?string | setRejectedTransactionId(?string rejectedTransactionId): void |
| `returnFee` | `?int` | Optional | Return Fee.<br><br>**Constraints**: `>= 0`, `<= 999999999` | getReturnFee(): ?int | setReturnFee(?int returnFee): void |
| `id` | `?string` | Optional | Transaction ACH Retry ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `retryTransactionId` | `?string` | Optional | Retry Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getRetryTransactionId(): ?string | setRetryTransactionId(?string retryTransactionId): void |
| `returnFeeTransactionId` | `?string` | Optional | Return Fee Transaction ID.<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getReturnFeeTransactionId(): ?string | setReturnFeeTransactionId(?string returnFeeTransactionId): void |
| `createdTs` | `?int` | Optional | Created Time Stamp | getCreatedTs(): ?int | setCreatedTs(?int createdTs): void |
| `createdUserId` | `?string` | Optional | User ID Created the register<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getCreatedUserId(): ?string | setCreatedUserId(?string createdUserId): void |
| `rejectedTransaction` | [`?Transaction`](../../doc/models/transaction.md) | Optional | - | getRejectedTransaction(): ?Transaction | setRejectedTransaction(?Transaction rejectedTransaction): void |
| `retryTransaction` | [`?Transaction`](../../doc/models/transaction.md) | Optional | - | getRetryTransaction(): ?Transaction | setRetryTransaction(?Transaction retryTransaction): void |
| `returnFeeTransaction` | [`?Transaction`](../../doc/models/transaction.md) | Optional | - | getReturnFeeTransaction(): ?Transaction | setReturnFeeTransaction(?Transaction returnFeeTransaction): void |
| `createdUser` | [`?User9`](../../doc/models/user-9.md) | Optional | - | getCreatedUser(): ?User9 | setCreatedUser(?User9 createdUser): void |
| `changelogs` | [`?(Changelog[])`](../../doc/models/changelog.md) | Optional | Changelog Information on `expand` | getChangelogs(): ?array | setChangelogs(?array changelogs): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "rejected_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "retry_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "return_fee_transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "created_ts": 1422040992,
  "created_user_id": "11e95f8ec39de8fbdb0a4f1a",
  "return_fee": 72,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

