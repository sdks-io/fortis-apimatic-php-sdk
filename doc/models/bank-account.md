
# Bank Account

The Bank Account.

*This model accepts additional fields of type array.*

## Structure

`BankAccount`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `routingNumber` | `?string` | Optional | Nine-digit Bank routing number.<br><br>**Constraints**: *Maximum Length*: `9` | getRoutingNumber(): ?string | setRoutingNumber(?string routingNumber): void |
| `accountNumber` | `?string` | Optional | Bank account number.<br><br>**Constraints**: *Maximum Length*: `17` | getAccountNumber(): ?string | setAccountNumber(?string accountNumber): void |
| `accountHolderName` | `?string` | Optional | Name on bank account.<br><br>**Constraints**: *Maximum Length*: `40` | getAccountHolderName(): ?string | setAccountHolderName(?string accountHolderName): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "routing_number": "011103093",
  "account_number": "01234567890123",
  "account_holder_name": "Bob Fairview",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

