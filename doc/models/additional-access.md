
# Additional Access

*This model accepts additional fields of type array.*

## Structure

`AdditionalAccess`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `merchantIcOptimization` | `?bool` | Optional | - | getMerchantIcOptimization(): ?bool | setMerchantIcOptimization(?bool merchantIcOptimization): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "merchant_ic_optimization": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

