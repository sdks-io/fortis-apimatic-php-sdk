
# Response Fullboarding

*This model accepts additional fields of type array.*

## Structure

`ResponseFullboarding`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | [`?string(Type30)`](../../doc/models/type-30.md) | Optional | - | getType(): ?string | setType(?string type): void |
| `data` | [`?Data9`](../../doc/models/data-9.md) | Optional | - | getData(): ?Data9 | setData(?Data9 data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "Fullboarding",
  "data": {
    "result": {
      "client_app_id": "client_app_id2",
      "dba_name": "dba_name4",
      "email": "email0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    "status": {
      "response_code": "response_code0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
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

