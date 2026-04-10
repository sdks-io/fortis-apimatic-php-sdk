
# Page

Use this field to specify paginate your results, by using page size and number. You can use one of the following methods:

> /endpoint?page={ "number": 1, "size": 50 }
> 
> /endpoint?page[number]=1&page[size]=50

*This model accepts additional fields of type array.*

## Structure

`Page`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `number` | `?int` | Optional | The current page number of the page to be retrieved.<br><br>**Constraints**: `>= 1` | getNumber(): ?int | setNumber(?int number): void |
| `size` | `?int` | Optional | The maximum number of records ta will be returned per page.<br><br>**Constraints**: `>= 1`, `<= 5000` | getSize(): ?int | setSize(?int size): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "number": 1,
  "size": 50,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

