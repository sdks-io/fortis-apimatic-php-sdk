
# V1 Wallet Provider Merchant Details Request

*This model accepts additional fields of type array.*

## Structure

`V1WalletProviderMerchantDetailsRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `merchantOrigin` | `string` | Required | Domain name where the Apple or Google pay button is or will be displayed. Full domain name including subdomain. | getMerchantOrigin(): string | setMerchantOrigin(string merchantOrigin): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "merchantOrigin": "dev.pay.site",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

