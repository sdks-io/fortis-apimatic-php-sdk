
# Batch Risk Config

Batch Risk Config

*This model accepts additional fields of type array.*

## Structure

`BatchRiskConfig`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `blindRefundTotalCount` | `?int` | Optional | Blind Refund Total Count<br><br>**Constraints**: `>= 0`, `<= 999999999` | getBlindRefundTotalCount(): ?int | setBlindRefundTotalCount(?int blindRefundTotalCount): void |
| `blindRefundMaxAmount` | `?int` | Optional | Blind Refund Max Amount<br><br>**Constraints**: `>= 0`, `<= 999999999` | getBlindRefundMaxAmount(): ?int | setBlindRefundMaxAmount(?int blindRefundMaxAmount): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "blind_refund_total_count": 110,
  "blind_refund_max_amount": 172,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

