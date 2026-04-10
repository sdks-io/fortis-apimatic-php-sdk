
# Response Error

*This model accepts additional fields of type array.*

## Structure

`ResponseError`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | `?string` | Optional | Message type | getType(): ?string | setType(?string type): void |
| `id` | `?string` | Optional | Unique identifier for this API call | getId(): ?string | setId(?string id): void |
| `statusCode` | `?int` | Optional | HTTP status code | getStatusCode(): ?int | setStatusCode(?int statusCode): void |
| `title` | `?string` | Optional | Error title | getTitle(): ?string | setTitle(?string title): void |
| `detail` | [`?Detail12`](../../doc/models/detail-12.md) | Optional | - | getDetail(): ?Detail12 | setDetail(?Detail12 detail): void |
| `meta` | `?array` | Optional | Object with additional error details | getMeta(): ?array | setMeta(?array meta): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "Error",
  "id": "c7f03d44-c966-4578-93ff-295f3ef6a467",
  "statusCode": 400,
  "title": "Bad Request",
  "detail": {
    "three_ds_server_trans_id": "three_ds_server_trans_id6",
    "acs_trans_id": "acs_trans_id8",
    "ds_trans_id": "ds_trans_id4",
    "error_code": "error_code4",
    "error_component": "error_component2",
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

