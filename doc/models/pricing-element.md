
# Pricing Element

Array of pricing items from template to be changed.

*This model accepts additional fields of type array.*

## Structure

`PricingElement`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `itemId` | `int` | Required | Item ID.<br><br>**Constraints**: `>= 0` | getItemId(): int | setItemId(int itemId): void |
| `itemValue` | `float` | Required | Item value.<br><br>**Constraints**: `>= 0` | getItemValue(): float | setItemValue(float itemValue): void |
| `itemTerm` | `int` | Required | Item term.<br><br>**Constraints**: `>= 0` | getItemTerm(): int | setItemTerm(int itemTerm): void |
| `itemDescription` | `?string` | Optional | Item desciption.<br><br>**Constraints**: *Maximum Length*: `100` | getItemDescription(): ?string | setItemDescription(?string itemDescription): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "item_id": 5,
  "item_value": 1.5,
  "item_term": 2,
  "item_description": "AVS fee.",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

