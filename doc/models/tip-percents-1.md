
# Tip Percents 1

*This model accepts additional fields of type array.*

## Structure

`TipPercents1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `percent1` | `?int` | Optional | field can only contain a value from 0 to 99, if 1 field is NULL, all fields must be null.<br><br>**Constraints**: `>= 0`, `<= 99` | getPercent1(): ?int | setPercent1(?int percent1): void |
| `percent2` | `?int` | Optional | field can only contain a value from 0 to 99, if 1 field is NULL, all fields must be null.<br><br>**Constraints**: `>= 0`, `<= 99` | getPercent2(): ?int | setPercent2(?int percent2): void |
| `percent3` | `?int` | Optional | field can only contain a value from 0 to 99, if 1 field is NULL, all fields must be null.<br><br>**Constraints**: `>= 0`, `<= 99` | getPercent3(): ?int | setPercent3(?int percent3): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "percent_1": 0,
  "percent_2": 2,
  "percent_3": 99,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

