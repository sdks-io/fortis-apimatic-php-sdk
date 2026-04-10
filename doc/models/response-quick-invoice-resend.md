
# Response Quick Invoice Resend

*This model accepts additional fields of type array.*

## Structure

`ResponseQuickInvoiceResend`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type61)`](../../doc/models/type-61.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data19`](../../doc/models/data-19.md) | Optional | - | getData(): ?Data19 | setData(?Data19 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "QuickInvoiceResend",
  "data": {
    "id": "id0",
    "email_log_id": "email_log_id2",
    "sms_log_id": "sms_log_id4",
    "success": false,
    "sms_success": false,
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

