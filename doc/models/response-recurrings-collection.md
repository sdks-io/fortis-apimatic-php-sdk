
# Response Recurrings Collection

*This model accepts additional fields of type array.*

## Structure

`ResponseRecurringsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type68)`](../../doc/models/type-68.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `list` | [`?(List11[])`](../../doc/models/list-11.md) | Optional | Resource Members | getList(): ?array | setList(?array list): void |
| `links` | [`?Links1`](../../doc/models/links-1.md) | Optional | - | getLinks(): ?Links1 | setLinks(?Links1 links): void |
| `pagination` | [`?Pagination1`](../../doc/models/pagination-1.md) | Optional | - | getPagination(): ?Pagination1 | setPagination(?Pagination1 pagination): void |
| `sort` | [`?Sort1`](../../doc/models/sort-1.md) | Optional | - | getSort(): ?Sort1 | setSort(?Sort1 sort): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "RecurringsCollection",
  "list": [
    {
      "account_vault_id": "account_vault_id8",
      "token_id": "token_id6",
      "contact_id": "contact_id2",
      "account_vault_api_id": "account_vault_api_id6",
      "token_api_id": "token_api_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_vault_id": "account_vault_id8",
      "token_id": "token_id6",
      "contact_id": "contact_id2",
      "account_vault_api_id": "account_vault_api_id6",
      "token_api_id": "token_api_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "account_vault_id": "account_vault_id8",
      "token_id": "token_id6",
      "contact_id": "contact_id2",
      "account_vault_api_id": "account_vault_api_id6",
      "token_api_id": "token_api_id2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "links": {
    "type": "Links",
    "first": "first0",
    "previous": "previous2",
    "next": "next2",
    "last": "last4",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "pagination": {
    "type": "Pagination",
    "total_count": 100,
    "page_count": 212,
    "page_number": 28,
    "page_size": 6,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "sort": {
    "type": "Sorting",
    "fields": [
      {
        "field": "field2",
        "order": "asc",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "field": "field2",
        "order": "asc",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      {
        "field": "field2",
        "order": "asc",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
    ],
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

