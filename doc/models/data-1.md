
# Data 1

*This model accepts additional fields of type array.*

## Structure

`Data1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `async` | [`?Async2`](../../doc/models/async-2.md) | Optional | - | getAsync(): ?Async2 | setAsync(?Async2 async): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "async": {
    "code": "00000038-0000-0000-0000-000000000000",
    "link": "link8",
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

