
# Additional Amount

*This model accepts additional fields of type array.*

## Structure

`AdditionalAmount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | `?array` | Optional | - | getType(): ?array | setType(?array type): void |
| `amount` | `?int` | Optional | The amount of additional amount. | getAmount(): ?int | setAmount(?int amount): void |
| `accountType` | `?array` | Optional | - | getAccountType(): ?array | setAccountType(?array accountType): void |
| `currency` | `?float` | Optional | Currency Code | getCurrency(): ?float | setCurrency(?float currency): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "amount": 10,
  "currency": 840.0,
  "type": {
    "key1": "val1",
    "key2": "val2"
  },
  "account_type": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

