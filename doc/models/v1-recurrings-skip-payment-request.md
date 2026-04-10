
# V1 Recurrings Skip Payment Request

*This model accepts additional fields of type array.*

## Structure

`V1RecurringsSkipPaymentRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `skipCount` | `int` | Required | Skip Count<br><br>**Constraints**: `>= 1`, `<= 99` | getSkipCount(): int | setSkipCount(int skipCount): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "skip_count": 7,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

