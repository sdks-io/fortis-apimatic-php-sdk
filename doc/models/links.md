
# Links

Pagination page links

*This model accepts additional fields of type array.*

## Structure

`Links`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type2)`](../../doc/models/type-2.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `first` | `?string` | Optional | Link to the first page | getFirst(): ?string | setFirst(?string first): void |
| `previous` | `?string` | Optional | Link to the previous page | getPrevious(): ?string | setPrevious(?string previous): void |
| `next` | `?string` | Optional | Link to the next page | getNext(): ?string | setNext(?string next): void |
| `last` | `?string` | Optional | Link to the last page | getLast(): ?string | setLast(?string last): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "first": "/v1/endpoint?page[size]=10&page[number]=1",
  "previous": "/v1/endpoint?page[size]=10&page[number]=5",
  "next": "/v1/endpoint?page[size]=10&page[number]=7",
  "last": "/v1/endpoint?page[size]=10&page[number]=42",
  "type": "Links",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

