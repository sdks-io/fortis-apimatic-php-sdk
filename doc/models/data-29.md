
# Data 29

*This model accepts additional fields of type array.*

## Structure

`Data29`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `id` | `?string` | Optional | Level 3 ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getId(): ?string | setId(?string id): void |
| `transactionId` | `?string` | Optional | Transaction ID<br><br>**Constraints**: *Pattern*: `^(([0-9a-fA-F\-]{24,36})\|(([0-9a-fA-F]{8})-(([0-9a-fA-F]{4}\-){3})([0-9a-fA-F]{12})))$` | getTransactionId(): ?string | setTransactionId(?string transactionId): void |
| `level3Data` | [`?Level3Data1`](../../doc/models/level-3-data-1.md) | Optional | - | getLevel3Data(): ?Level3Data1 | setLevel3Data(?Level3Data1 level3Data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "id": "11e95f8ec39de8fbdb0a4f1a",
  "transaction_id": "11e95f8ec39de8fbdb0a4f1a",
  "level3_data": {
    "destination_country_code": "destination_country_code4",
    "duty_amount": 182,
    "freight_amount": 60,
    "national_tax": 999999998900,
    "sales_tax": 999999998900,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

