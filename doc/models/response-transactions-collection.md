
# Response Transactions Collection

*This model accepts additional fields of type array.*

## Structure

`ResponseTransactionsCollection`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type117)`](../../doc/models/type-117.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `list` | [`?(List18[])`](../../doc/models/list-18.md) | Optional | Resource Members | getList(): ?array | setList(?array list): void |
| `links` | [`?Links1`](../../doc/models/links-1.md) | Optional | - | getLinks(): ?Links1 | setLinks(?Links1 links): void |
| `pagination` | [`?Pagination1`](../../doc/models/pagination-1.md) | Optional | - | getPagination(): ?Pagination1 | setPagination(?Pagination1 pagination): void |
| `sort` | [`?Sort1`](../../doc/models/sort-1.md) | Optional | - | getSort(): ?Sort1 | setSort(?Sort1 sort): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "TransactionsCollection",
  "list": [
    {
      "additional_amounts": [
        {
          "type": {
            "key1": "val1",
            "key2": "val2"
          },
          "amount": 6,
          "account_type": {
            "key1": "val1",
            "key2": "val2"
          },
          "currency": 154.64,
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "billing_address": {
        "city": "city2",
        "state": "state6",
        "postal_code": "postal_code0",
        "street": "street8",
        "phone": "phone2",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "checkin_date": "checkin_date4",
      "checkout_date": "checkout_date6",
      "clerk_number": "clerk_number6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "additional_amounts": [
        {
          "type": {
            "key1": "val1",
            "key2": "val2"
          },
          "amount": 6,
          "account_type": {
            "key1": "val1",
            "key2": "val2"
          },
          "currency": 154.64,
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "billing_address": {
        "city": "city2",
        "state": "state6",
        "postal_code": "postal_code0",
        "street": "street8",
        "phone": "phone2",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "checkin_date": "checkin_date4",
      "checkout_date": "checkout_date6",
      "clerk_number": "clerk_number6",
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

