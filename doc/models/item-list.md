
# Item List

*This model accepts additional fields of type array.*

## Structure

`ItemList`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `name` | `?string` | Optional | Item's Name, must be unique on the list<br><br>**Constraints**: *Maximum Length*: `100` | getName(): ?string | setName(?string name): void |
| `amount` | `?int` | Optional | Item's Amount<br><br>**Constraints**: `>= -999999999`, `<= 999999999` | getAmount(): ?int | setAmount(?int amount): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "name": "Bread",
  "amount": 2015,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

