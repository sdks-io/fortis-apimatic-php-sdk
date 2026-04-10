
# Balance

*This model accepts additional fields of type array.*

## Structure

`Balance`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `amountType` | `?string` | Optional | The type of amount balance | getAmountType(): ?string | setAmountType(?string amountType): void |
| `accountType` | `?string` | Optional | The type of account balance | getAccountType(): ?string | setAccountType(?string accountType): void |
| `amount` | `?int` | Optional | The amount of balance | getAmount(): ?int | setAmount(?int amount): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "amount": 1000,
  "amount_type": "amount_type4",
  "account_type": "account_type6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

