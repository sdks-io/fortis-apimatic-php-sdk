
# Kyc Response Object

Array of KYC response objects.

*This model accepts additional fields of type array.*

## Structure

`KycResponseObject`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `value` | `string` | Required | KYC object value. | getValue(): string | setValue(string value): void |
| `type` | `string` | Required | KYC oject type.<br><br>**Constraints**: *Maximum Length*: `32` | getType(): string | setType(string type): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "value": "KYC value.",
  "type": "KYC type",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

