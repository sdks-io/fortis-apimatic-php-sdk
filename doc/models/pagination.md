
# Pagination

Pagination info

*This model accepts additional fields of type array.*

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type3)`](../../doc/models/type-3.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `totalCount` | `?int` | Optional | Total records count | getTotalCount(): ?int | setTotalCount(?int totalCount): void |
| `pageCount` | `?int` | Optional | Total page count | getPageCount(): ?int | setPageCount(?int pageCount): void |
| `pageNumber` | `?int` | Optional | Current page | getPageNumber(): ?int | setPageNumber(?int pageNumber): void |
| `pageSize` | `?int` | Optional | Page size | getPageSize(): ?int | setPageSize(?int pageSize): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "total_count": 423,
  "page_count": 42,
  "page_number": 6,
  "page_size": 10,
  "type": "Pagination",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

