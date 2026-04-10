
# Meta

*This model accepts additional fields of type array.*

## Structure

`Meta`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `details` | [`?(Detail[])`](../../doc/models/detail.md) | Optional | Error detail | getDetails(): ?array | setDetails(?array details): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "details": [
    {
      "message": "message0",
      "path": [
        "path6"
      ],
      "type": "type0",
      "context": {
        "key": "key2",
        "label": "label2",
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
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

