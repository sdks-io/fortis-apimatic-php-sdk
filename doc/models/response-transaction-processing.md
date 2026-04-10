
# Response Transaction Processing

*This model accepts additional fields of type array.*

## Structure

`ResponseTransactionProcessing`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type5)`](../../doc/models/type-5.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data1`](../../doc/models/data-1.md) | Optional | - | getData(): ?Data1 | setData(?Data1 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "TransactionProcessing",
  "data": {
    "async": {
      "code": "00000038-0000-0000-0000-000000000000",
      "link": "link8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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

