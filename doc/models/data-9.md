
# Data 9

*This model accepts additional fields of type array.*

## Structure

`Data9`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `result` | [`?Result`](../../doc/models/result.md) | Optional | - | getResult(): ?Result | setResult(?Result result): void |
| `status` | [`?Status5`](../../doc/models/status-5.md) | Optional | - | getStatus(): ?Status5 | setStatus(?Status5 status): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
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
}
```

