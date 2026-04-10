
# Response Payment Card Reader Token

*This model accepts additional fields of type array.*

## Structure

`ResponsePaymentCardReaderToken`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type58)`](../../doc/models/type-58.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data17`](../../doc/models/data-17.md) | Optional | - | getData(): ?Data17 | setData(?Data17 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "PaymentCardReaderToken",
  "data": {
    "token": "token4",
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

