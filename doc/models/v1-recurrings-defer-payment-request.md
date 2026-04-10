
# V1 Recurrings Defer Payment Request

*This model accepts additional fields of type array.*

## Structure

`V1RecurringsDeferPaymentRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `deferCount` | `int` | Required | Defer Count<br><br>**Constraints**: `>= 1`, `<= 99` | getDeferCount(): int | setDeferCount(int deferCount): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "defer_count": 5,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

