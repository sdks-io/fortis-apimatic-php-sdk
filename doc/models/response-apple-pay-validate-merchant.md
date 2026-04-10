
# Response Apple Pay Validate Merchant

*This model accepts additional fields of type array.*

## Structure

`ResponseApplePayValidateMerchant`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type136)`](../../doc/models/type-136.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data37`](../../doc/models/data-37.md) | Optional | - | getData(): ?Data37 | setData(?Data37 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "ApplePayValidateMerchant",
  "data": {
    "merchantSession": "merchantSession0",
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

